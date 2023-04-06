---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ServicePrincipalsRequestBuilderGetRequestConfiguration(
request_config = ServicePrincipalsRequestBuilderGetRequestConfiguration(query_params=query_params = ServicePrincipalsRequestBuilderGetQueryParameters()
query_params.filter = "startswith(displayName,%20'a')"
query_params.count = true
query_params.top = 1
query_params.orderby = ["displayName"]

)
query_params = ServicePrincipalsRequestBuilderGetQueryParameters()
query_params.filter = "startswith(displayName,%20'a')"
query_params.count = true
query_params.top = 1
query_params.orderby = ["displayName"]

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.servicePrincipals.get(request_config, headers=request_config)


```