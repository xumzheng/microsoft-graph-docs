---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ServicePrincipalRequestBuilderGetRequestConfiguration()

query_params = ServicePrincipalRequestBuilderGetQueryParameters()
query_params.select = ["customSecurityAttributes"]

request_config.queryParameters = query_params


result = await client.servicePrincipalsById('servicePrincipal-id').get(request_config)


```