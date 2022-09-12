---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new GroupLifecyclePolicy
{
	GroupLifetimeInDays = 100,
	ManagedGroupTypes = "Selected",
	AlternateNotificationEmails = "admin@contoso.com",
};
var result = await graphClient.GroupLifecyclePolicies.PostAsync(requestBody);


```