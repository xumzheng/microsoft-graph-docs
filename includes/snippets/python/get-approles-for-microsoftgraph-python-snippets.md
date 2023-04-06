---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ServicePrincipalsRequestBuilderGetRequestConfiguration(
request_config = ServicePrincipalsRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "displayName eq 'Microsoft Graph'"
params['select'] = ["id","displayName","appId","appRoles"]
)


result = await client.servicePrincipals.get(request_config, headers=request_config)


```