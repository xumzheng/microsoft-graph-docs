---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ApplicationsRequestBuilderGetRequestConfiguration(
query_params = ApplicationsRequestBuilderGetQueryParameters()
query_params.search = "\"displayName:Browser\""

)


result = await client.applications.get(request_config)


```