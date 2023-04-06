---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = ServicePrincipalsRequestBuilderGetRequestConfiguration(
request_configuration = ServicePrincipalsRequestBuilderGetRequestConfiguration(query_params=query_params = ServicePrincipalsRequestBuilderGetQueryParameters()
query_params['filter'] = "displayName eq 'Microsoft Graph'"
query_params['select'] = ["id","displayName","appId","oauth2PermissionScopes"]

)
query_params = ServicePrincipalsRequestBuilderGetQueryParameters()
query_params['filter'] = "displayName eq 'Microsoft Graph'"
query_params['select'] = ["id","displayName","appId","oauth2PermissionScopes"]

)


result = await client.servicePrincipals.get(request_configuration)


```