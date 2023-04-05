---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = EventsRequestBuilderGetRequestConfiguration(
query_params = EventsRequestBuilderGetQueryParameters()
query_params.select = ["subject","body","bodyPreview"]

headers = [
'Prefer' => 'outlook.body-content-type="text"',
]

)


result = await client.me.events.get(request_config)


```