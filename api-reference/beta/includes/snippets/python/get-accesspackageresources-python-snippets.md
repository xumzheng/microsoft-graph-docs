---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AccessPackageResourcesRequestBuilderGetRequestConfiguration(
request_config = AccessPackageResourcesRequestBuilderGetRequestConfiguration(query_params=query_params = AccessPackageResourcesRequestBuilderGetQueryParameters()
query_params.filter = "resourceType eq 'Application'"
query_params.expand = ["accessPackageResourceScopes"]

)
query_params = AccessPackageResourcesRequestBuilderGetQueryParameters()
query_params.filter = "resourceType eq 'Application'"
query_params.expand = ["accessPackageResourceScopes"]

)


result = await client.identityGovernance.entitlementManagement.accessPackageCatalogs_by_id('accessPackageCatalog-id').accessPackageResources.get(request_config, headers=request_config)


```