---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = EventsRequestBuilderGetRequestConfiguration(
request_config = EventsRequestBuilderGetRequestConfiguration(query_params=query_params = EventsRequestBuilderGetQueryParameters()
query_params.select = ["subject","body","bodyPreview","organizer","attendees","start","end","location"]

)
query_params = EventsRequestBuilderGetQueryParameters()
query_params.select = ["subject","body","bodyPreview","organizer","attendees","start","end","location"]

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.me.events.get(request_config, headers=request_config)


```