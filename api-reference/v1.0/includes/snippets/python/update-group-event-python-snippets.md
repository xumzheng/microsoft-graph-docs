---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Event();
location = Location();
location.setDisplayName('Conf Room 2');


requestBody.setLocation($location);


requestResult = graphServiceClient.groupsById('group-id').calendar().eventsById('event-id').patch(requestBody);


```