---
title: "Education Graph API Best Practices"
description: "Provides best practices for developers on how best to use EDU assignments graph apis."
ms.localizationpriority: medium
author: "sharad-sharma-msft"
ms.prod: "education"
doc_type: conceptualPageType
---

# Education Graph API Best Practices
This article walks through the best practices for using the Assignments .NET SDK. Following these practices, will help improve your latency, availability, and boost overall performance. 

## Pre-condition
Before you delve into these best practices, it is important to make sure that you are familiar with-
1. Graph SDK [Overview](/graph/sdks/sdks-overview)
2. General best practices for Microsoft Graph. The general best practices are listed [here](https://github.com/microsoftgraph/microsoft-graph-docs/blob/main/concepts/best-practices-concept.md)

## Checklist

| Checked | Topic | Details/Links |
|--|--|--|
| |SDK Version | Always using the [latest version] (https://www.nuget.org/packages/Microsoft.Graph.Core) of the Graph SDK available for optimal performance. |
| |Singleton Client | Use a single instance of `GraphServiceClient` for the lifetime of your application for better performance
| | CPU | You may run into connectivity/availability issues due to lack of resources on your client machine. Monitor your CPU utilization on nodes running the graph client and scale up/out if usage is very high.
| |Hosting | Use Windows 64-bit host processing for best performance, whenever possible.
| |Networking | If using a virtual machine to run your application, enable [Accelerated Networking] (/azure/virtual-network/create-vm-accelerated-networking-powershell) on your VM to help with bottlenecks due to high traffic and reduce latency or CPU jitter. You might also want to consider using a higher end Virtual Machine where the max CPU usage is under 70%.
| |Use Async/Await |Avoid blocking calls: `Task.Result`, `Task.Wait`, and `Task.GetAwaiter().GetResult()`. The entire call stack is asynchronous in order to benefit from [async/await](/dotnet/csharp/programming-guide/concepts/async/) patterns. Many synchronous blocking calls lead to [Thread Pool starvation](/archive/blogs/vancem/diagnosing-net-core-threadpool-starvation-with-perfview-why-my-service-is-not-saturating-all-cores-or-seems-to-stall) and degraded response times.
| |End-to-End Timeouts | To get end-to-end timeouts, you'll need to use both `RequestTimeout` and `CancellationToken` parameters.
| |Retry Logic | A transient error is an error that has an underlying cause that soon resolves itself. Applications that connect to your database should be built to expect these transient errors. To handle them, implement retry logic in your code instead of surfacing them to users as application errors. The SDK has built-in logic to handle these transient failures on retryable requests like read or query operations. The SDK will not retry on writes for transient failures as writes are not idempotent. The SDK does allow users to configure retry logic for throttles. |
| |Performance Testing Backoffs | When performing testing on your application, you should implement backoffs at `RetryAfter` intervals. Respecting the backoff helps ensure that you'll spend a minimal amount of time waiting between retries.


## Latency
Here are some suggestions to improve your latency.

### Use $select whenever possible
By default, Assignments APIs return a fixed set of properties on GET requests. For example, see the properties returned on an assignment GET by default:

GET Request:
```
GET https://graph.microsoft.com/v1.0/education/me/assignments
```

GET Response:
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/me/assignments",
    "value": [
        {
            "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "displayName": "Expand options 3.1",
            "closeDateTime": "2021-11-19T07:59:00Z",
            "dueDateTime": "2021-11-19T07:59:00Z",
            "assignDateTime": null,
            "assignedDateTime": null,
            "allowLateSubmissions": false,
            "resourcesFolderUrl": null,
            "createdDateTime": "2021-11-10T23:56:21.1575202Z",
            "lastModifiedDateTime": "2021-11-17T16:00:30.0523446Z",
            "allowStudentsToAddResourcesToSubmission": false,
            "status": "published",
            "notificationChannelUrl": null,
            "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%2272a7baec-c3e9-4213-a850-f62de0adad5f%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%223b870c07-21fe-47fb-8562-cdd6f2c281d6%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
            "addToCalendarAction": "none",
            "addedStudentAction": "none",
            "id": "3b870c07-21fe-47fb-8562-cdd6f2c281d6",
            "instructions": null,
            "grading": null,
            "assignTo": null,
            "createdBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            },
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            }
        },
        {
            "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "displayName": "Expand options 4",
            "closeDateTime": null,
            "dueDateTime": "2021-11-12T07:59:00Z",
            "assignDateTime": null,
            "assignedDateTime": null,
            "allowLateSubmissions": true,
            "resourcesFolderUrl": null,
            "createdDateTime": "2021-11-10T23:58:41.5064997Z",
            "lastModifiedDateTime": "2021-11-10T23:58:41.5304842Z",
            "allowStudentsToAddResourcesToSubmission": false,
            "status": "draft",
            "notificationChannelUrl": null,
            "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%2272a7baec-c3e9-4213-a850-f62de0adad5f%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%2234ab8c17-eaae-4996-9c04-53696934e6ff%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
            "addToCalendarAction": "none",
            "addedStudentAction": "none",
            "id": "34ab8c17-eaae-4996-9c04-53696934e6ff",
            "instructions": null,
            "grading": null,
            "assignTo": null,
            "createdBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            },
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            }
        }
    ]
}

```

You see that all the entity defined properties are returned, as well as all of the application-defined properties.

In many scenarios, an application only cares about a subset of the properties on any item at a given time. In that case, you should specify the $select query parameter and provide the subset of properties the application's logic requires at that time.

For example, for the item above, let's say for the application's scenario, it is only interested in displayName, dueDateTime, and CreatedDateTime. You can specify those three properties in the $select query parameter.

GET with $select request:

```
GET https://graph.microsoft.com/v1.0/education/me/assignments/?$select=dueDateTime,displayName
```

GET with $select response:

```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/me/assignments",
    "value": [
        {
            "displayName": "Expand options 3.1",
            "dueDateTime": "2021-11-19T07:59:00Z"
        },
        {
            "displayName": "Expand options 4",
            "dueDateTime": "2021-11-12T07:59:00Z"
         }
    ]
}
```

You see that the only properties that are returned are the one selected.

This helps performance in the following ways:
1.
Can reduce the calls we make to our underlying storage to retrieve the assignment (especially if the application takes advantage of large properties and omits them from $select query parameter in certain scenarios).
2.
Reduces COGs for JSON deserialization in the application calling assignments.
3.
Less bits to transmit over the wire.

### When using $filter, also specify $orderby
When a GET call with a $filter query parameter also has a $orderby, and the $orderby contains at least one property from the $filter, we will generate an index in our underlying database so subsequent GETs will return more quickly. So, if an application has a filter clause like this:

.../assignments/?$filter=status ne 'draft'

You can generate an index for that filter by adding the ordering clause:

.../assignments/?$filter=status ne 'draft'&$orderby=displayName

The performance gain is amortized; the first time an application makes the $filter/$orderby query, the index needs to be generated, so the request will take longer than if just the $filter query parameter is used. However, all subsequent calls will be faster than if just the filter was passed.

We allow filtering and ordering on select properties.

## Throttling
Your application calls the assignments service. In some cases, you might need to make calls in the context of e.g., say a lot of students and/or resources. This can cause a spike in service traffic. In order to safeguard itself against such spikes and to make sure service remains available to all callers, the service will throttle this specific caller. See our [throttling limits](/graph/throttling-limits#assignment-service-limits).

In order to make sure you build smooth user experience; the application need to ensure it is not generating lot of calls in the short span of time. You can implement a concurrency control using one of the following mechanisms-
- [ConcurrentQueue](/dotnet/api/system.collections.concurrent.concurrentqueue-1)
  The basic idea is to put the work onto a queue and then have multiple threads reading off that queue. This is a nice simple approach, but it does require us to remember to lock the queue as it will be accessed by multiple threads. In this example I'm using ConcurrentQueue to give us thread safety.
- [SemaphoreSlim](/dotnet/api/system.threading.semaphoreslim)
  Use a SemaphoreSlim with an initialCount equal to the maximum number of threads. Then you use WaitAsync to wait until it's OK to queue up another.
- [Parallel.ForEach](/dotnet/api/system.threading.tasks.parallel.foreach)
   You can simply specify the `MaxDegreeOfParallelism` and then provide an Action to perform on each item in your `IEnumerable`
- [Polly Bulkhead Policy](https://github.com/App-vNext/Polly/wiki/Bulkhead)
  A bulkhead policy restricts the number of concurrent calls that can be made, and optionally allows you to queue up calls that exceed that number.

These patterns allow you to use a constrained number of threads to work through a batch of jobs.

### How to avoid excessive throttling?
Often times excessive throttling is self-inflicted injury i.e. you are calling the service more often than service would want you to call it. The assignment service will send Retry-After header in the response with recommended delay in making subsequent calls. Please consume the value in this header and wait for the recommended interval before making the next API call from your application.

## CancellationToken
Whether you’re doing async work or not, accepting a CancellationToken as a parameter to your method is a great pattern for allowing your caller to express lost interest in the result.

Supporting cancelable operations comes with a little bit of extra responsibility on your part.

1. __Know when you’ve passed the point of no cancellation. __
_Don’t_ cancel if you’ve already incurred side-effects that your method isn’t prepared to revert on the way out that would leave you in an inconsistent state. So, if you’ve done some work, and have a lot more to do, and the token is cancelled, you must only cancel when and if you can do so leaving objects in a valid state. This may mean that you have to finish the large amount of work, or undo all your previous work (i.e., revert the side-effects) or find a convenient place that you can stop halfway through but in a valid condition, before then throwing `OperationCanceledException`. In other words, the caller must be able to recover to a known consistent state after cancelling your work or realize that cancellation was not responded to and that the caller then must decide whether to accept the work or revert its successful completion on its own.

2. __Propagate your CancellationToken__ to all the methods you call that accept one, except after the “point of no cancellation” referred to in the previous point. In fact, if your method mostly orchestrates calls to other methods that themselves take CancellationTokens, you may find that you don’t personally have to call `CancellationToken.ThrowIfCancellationRequested()` at all, since the async methods you’re calling will generally do it for you.
3. __Don’t throw `OperationCanceledException` after you’ve completed the work__, just because the token was signaled. Return a successful result and let the caller decide what to do next. The caller can’t assume you’re cancellable at a given point anyway, so they have to be prepared for a successful result even upon cancellation.
4. __Input validation__ can certainly go ahead of cancellation checks (since that helps highlight bugs in the calling code).
5. __Consider not checking the token at all__ if your work is very quick, or you propagate it to the methods you call. That said, calling `CancellationToken.ThrowIfCancellationRequested()` is pretty lightweight so don’t think too hard about this one unless you see it on perf traces.
6. __Check `CancellationToken.CanBeCanceled`__ when you can do your work more efficiently if you can assume you’ll never be canceled. CanBeCanceled returns false for `CancellationToken.None`, and in the future possibly for other cases as well.
### Optional CancellationToken parameter
If you want to accept CancellationToken but want to make it optional, you can do so with syntax such as this:
```
public Task SomethingExpensiveAsync(CancellationToken cancellationToken = default (CancellationToken))
{
  // don't worry about NullReferenceException if the
  // caller omitted the argument because it's a struct.
  cancellationToken.ThrowIfCancellationRequested();
}
```

It’s a good idea to only make your CancellationToken parameters optional in your public API (if you have one) and leave them as required parameters everywhere else. This really helps to ensure that you intentionally propagate your CancellationTokens through all the methods you call (number 2 above). But of course, remember to switch to passing CancellationToken.None once you pass the point of no cancellation.

It’s also a good API pattern to keep your CancellationToken as the last parameter your method accepts. This fits nicely with optional parameters anyway since they have to show up after any required parameters.

### Handling cancellation exceptions
If you’ve experienced cancellation before, you’ve probably noticed a couple of types of these exceptions: TaskCanceledException and OperationCanceledException. TaskCanceledException derives from OperationCanceledException. That means when writing your catch blocks that deal with the fallout of a canceled operation, you should catch OperationCanceledException. If you catch TaskCanceledException you may let certain cancellation occurrences slip through your catch blocks (and possibly crash your app).

```
async Task UserSubmitClickAsync(CancellationToken cancellationToken)
{
  try
  {
    await SendResultAsync(cancellationToken);
  }
  catch (OperationCanceledException ex) // includes TaskCanceledException
  {
    MessageBox.Show("Your submission was canceled.");
  }
}
```

If your cancelable method is in between other cancelable operations, you may need to perform clean up when canceled. When doing so, you can use the above catch block, but be sure to rethrow properly:

```
async Task SendResultAsync(CancellationToken cancellationToken)
{
  try
  {
    await httpClient.SendAsync(form, cancellationToken);
  }
  catch (OperationCanceledException ex)
  {
    // perform your cleanup
    form.Dispose();

    // rethrow exception so caller knows you've canceled.
    // DON'T "throw ex;" because that stomps on
    // the Exception.StackTrace property.
    throw;
  }
}
```

## FAQ
### What to do we if application is seeing 400 (bad request) status code in the service requests?
The application developer needs to review the assignment service graph documentation carefully. You are likely missing some property or the value of one or more property related to entity in question is wrong.

### What we do if we see Internal Server error?
If anytime you see 500 (Internal Server error), Please report it to us.

