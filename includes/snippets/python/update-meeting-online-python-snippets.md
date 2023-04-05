---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Event()
request_body.setIsOnlineMeeting(true)

request_body.setOnlineMeetingProvider(OnlineMeetingProviderType('teamsforbusiness'))



result = await client.me_eventsby_id('event-id').patch(request_body)


```