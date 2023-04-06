---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = EventRequestBuilderGetRequestConfiguration(
request_configuration = EventRequestBuilderGetRequestConfiguration(query_params=query_params = EventRequestBuilderGetQueryParameters()
query_params['select'] = ["isOnlineMeeting","onlineMeetingProvider","onlineMeeting"]

)
query_params = EventRequestBuilderGetQueryParameters()
query_params['select'] = ["isOnlineMeeting","onlineMeetingProvider","onlineMeeting"]

)


result = await client.me.events_by_id('event-id').get(request_configuration)


```