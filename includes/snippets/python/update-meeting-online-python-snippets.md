---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Event();
requestBody.setIsOnlineMeeting(true);

requestBody.setOnlineMeetingProvider(OnlineMeetingProviderType('teamsforbusiness'));



result = await client.me().eventsById('event-id').patch(requestBody);


```