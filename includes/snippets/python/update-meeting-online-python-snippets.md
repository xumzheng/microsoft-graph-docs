---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Event()
request_body.isOnlineMeeting = true

request_body.OnlineMeetingProvider(OnlineMeetingProviderType('teamsforbusiness'))



request_configuration = EventRequestBuilderPatchRequestConfiguration(
)


result = await client.me.events_by_id('event-id').patch(request_body = request_body)


```