---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = AppRoleAssignedResourcesRequestBuilder.AppRoleAssignedResourcesRequestBuilderGetQueryParameters(
				select = ["displayName","accountEnabled","servicePrincipalType","signInAudience"],
)

request_configuration = AppRoleAssignedResourcesRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
headers = {
								'ConsistencyLevel' : "eventual",
}

)


result = await client.me.appRoleAssignedResources.get(request_configuration = request_configuration)


```