---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = EventRequestBuilder.EventRequestBuilderGetQueryParameters(
				select = ["subject","body","bodyPreview","organizer","attendees","start","end","location","hideAttendees"],
)

request_configuration = EventRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
headers = {
								'Prefer' : "outlook.timezone=\"Pacific Standard Time\"",
}

)


result = await client.me.events_by_id('event-id').get(request_configuration = request_configuration)


```