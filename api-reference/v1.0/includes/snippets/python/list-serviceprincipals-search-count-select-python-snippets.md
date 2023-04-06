---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ServicePrincipalsRequestBuilderGetRequestConfiguration(
request_config = ServicePrincipalsRequestBuilderGetRequestConfiguration(query_params=params['search'] = "\"displayName:Team\""
params['count'] = true
params['select'] = ["accountEnabled","displayName","publisherName","servicePrincipalType","signInAudience"]
)
headers['ConsistencyLevel'] = "eventual"


result = await client.servicePrincipals.get(request_config, headers=request_config)


```