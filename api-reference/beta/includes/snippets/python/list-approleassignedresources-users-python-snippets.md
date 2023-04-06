---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = AppRoleAssignedResourcesRequestBuilderGetRequestConfiguration(
request_configuration = AppRoleAssignedResourcesRequestBuilderGetRequestConfiguration(query_params=query_params = AppRoleAssignedResourcesRequestBuilderGetQueryParameters()
query_params['select'] = ["displayName","accountEnabled","servicePrincipalType","signInAudience"]

)
query_params = AppRoleAssignedResourcesRequestBuilderGetQueryParameters()
query_params['select'] = ["displayName","accountEnabled","servicePrincipalType","signInAudience"]

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.me.appRoleAssignedResources.get(request_configuration)


```