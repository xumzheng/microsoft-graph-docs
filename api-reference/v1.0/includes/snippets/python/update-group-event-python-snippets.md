---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Event();
location = Location();
location.setDisplayName('Conf Room 2');


requestBody.setLocation($location);


result = awaitclient.groupsById('group-id').calendar().eventsById('event-id').patch(requestBody);


```