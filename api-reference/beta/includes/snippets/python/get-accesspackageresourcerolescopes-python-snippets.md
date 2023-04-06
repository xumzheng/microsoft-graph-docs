---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AccessPackageRequestBuilderGetRequestConfiguration(
request_config = AccessPackageRequestBuilderGetRequestConfiguration(query_params=query_params = AccessPackageRequestBuilderGetQueryParameters()
query_params.expand = ["accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)"]

)
query_params = AccessPackageRequestBuilderGetQueryParameters()
query_params.expand = ["accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)"]

)


result = await client.identityGovernance.entitlementManagement.accessPackages_by_id('accessPackage-id').get(request_config, headers=request_config)


```