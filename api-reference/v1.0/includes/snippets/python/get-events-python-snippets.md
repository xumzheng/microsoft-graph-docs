---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = EventsRequestBuilderGetRequestConfiguration(
query_params = EventsRequestBuilderGetQueryParameters()
query_params.select = ["subject","body","bodyPreview","organizer","attendees","start","end","location"]

headers = [
'Prefer' => 'outlook.timezone="Pacific Standard Time"',
]

)


result = await client.me.events.get(request_config)


```