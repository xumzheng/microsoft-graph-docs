---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Event()
request_body.setIsOnlineMeeting(true)

request_body.setOnlineMeetingProvider(OnlineMeetingProviderType('teamsforbusiness'))


request_config = EventRequestBuilderPatchRequestConfiguration(
request_config = EventRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.me.events_by_id('event-id').patch(request_body, headers=)


```