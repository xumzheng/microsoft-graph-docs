---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = EventRequestBuilderGetRequestConfiguration(
request_configuration = EventRequestBuilderGetRequestConfiguration(query_params=query_params = EventRequestBuilderGetQueryParameters()
query_params['select'] = ["subject","body","bodyPreview","organizer","attendees","start","end","location","hideAttendees"]

)
query_params = EventRequestBuilderGetQueryParameters()
query_params['select'] = ["subject","body","bodyPreview","organizer","attendees","start","end","location","hideAttendees"]

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.me.events_by_id('event-id').get(request_configuration)


```