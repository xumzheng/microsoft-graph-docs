---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ServicePrincipalsRequestBuilderGetRequestConfiguration(
query_params = ServicePrincipalsRequestBuilderGetQueryParameters()
query_params.filter = "appId eq '00000002-0000-0000-c000-000000000000'"

)


result = await client.servicePrincipals.get(request_config)


```