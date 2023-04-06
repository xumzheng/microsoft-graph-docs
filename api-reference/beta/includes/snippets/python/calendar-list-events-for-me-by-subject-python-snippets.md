---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = EventsRequestBuilderGetRequestConfiguration(
request_config = EventsRequestBuilderGetRequestConfiguration(query_params=query_params = EventsRequestBuilderGetQueryParameters()
query_params.filter = "startsWith(subject,'All')"

)
query_params = EventsRequestBuilderGetQueryParameters()
query_params.filter = "startsWith(subject,'All')"

)


result = await client.me.calendar.events.get(request_config, headers=request_config)


```