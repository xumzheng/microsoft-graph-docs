---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Event();
requestBody.setIsOnlineMeeting(true);

requestBody.setOnlineMeetingProvider(OnlineMeetingProviderType('teamsforbusiness'));



requestResult = graphServiceClient.me().eventsById('event-id').patch(requestBody);


```