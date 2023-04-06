---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = ServicePrincipalRequestBuilderGetRequestConfiguration(
request_configuration = ServicePrincipalRequestBuilderGetRequestConfiguration(query_params=query_params = ServicePrincipalRequestBuilderGetQueryParameters()
query_params['select'] = ["id","appId","displayName","appRoles","oauth2PermissionScopes"]

)
query_params = ServicePrincipalRequestBuilderGetQueryParameters()
query_params['select'] = ["id","appId","displayName","appRoles","oauth2PermissionScopes"]

)


result = await client.servicePrincipals_by_id('servicePrincipal-id').get(request_configuration)


```