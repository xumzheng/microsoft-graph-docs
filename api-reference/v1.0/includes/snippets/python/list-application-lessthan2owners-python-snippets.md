---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ApplicationsRequestBuilderGetRequestConfiguration(
request_config = ApplicationsRequestBuilderGetRequestConfiguration(query_params=query_params = ApplicationsRequestBuilderGetQueryParameters()
query_params.filter = "owners/$count eq 0 or owners/$count eq 1"
query_params.count = true
query_params.select = ["id","displayName"]

)
query_params = ApplicationsRequestBuilderGetQueryParameters()
query_params.filter = "owners/$count eq 0 or owners/$count eq 1"
query_params.count = true
query_params.select = ["id","displayName"]

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.applications.get(request_config, headers=request_config)


```