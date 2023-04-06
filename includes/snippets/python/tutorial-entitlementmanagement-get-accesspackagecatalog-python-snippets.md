---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = AccessPackageCatalogsRequestBuilderGetRequestConfiguration(
request_configuration = AccessPackageCatalogsRequestBuilderGetRequestConfiguration(query_params=query_params = AccessPackageCatalogsRequestBuilderGetQueryParameters()
query_params['filter'] = "(displayName eq 'General')"

)
query_params = AccessPackageCatalogsRequestBuilderGetQueryParameters()
query_params['filter'] = "(displayName eq 'General')"

)


result = await client.identityGovernance.entitlementManagement.accessPackageCatalogs.get(request_configuration)


```