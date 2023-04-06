---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = EventsRequestBuilderGetRequestConfiguration(
request_configuration = EventsRequestBuilderGetRequestConfiguration(query_params=query_params = EventsRequestBuilderGetQueryParameters()
query_params['filter'] = "startsWith(subject,'All')"

)
query_params = EventsRequestBuilderGetQueryParameters()
query_params['filter'] = "startsWith(subject,'All')"

)


result = await client.me.calendar.events.get(request_configuration)


```