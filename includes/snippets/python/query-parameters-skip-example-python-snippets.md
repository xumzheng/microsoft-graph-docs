---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = EventsRequestBuilderGetRequestConfiguration(
request_configuration = EventsRequestBuilderGetRequestConfiguration(query_params=query_params = EventsRequestBuilderGetQueryParameters()
query_params['orderby'] = ["createdDateTime"]
query_params['skip'] = 20

)
query_params = EventsRequestBuilderGetQueryParameters()
query_params['orderby'] = ["createdDateTime"]
query_params['skip'] = 20

)


result = await client.me.events.get(request_configuration)


```