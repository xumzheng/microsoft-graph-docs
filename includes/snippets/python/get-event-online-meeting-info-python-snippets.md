---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = EventRequestBuilderGetRequestConfiguration(
request_config = EventRequestBuilderGetRequestConfiguration(query_params=params['select'] = ["isOnlineMeeting","onlineMeetingProvider","onlineMeeting"]
)


result = await client.me.events_by_id('event-id').get(request_config, headers=request_config)


```