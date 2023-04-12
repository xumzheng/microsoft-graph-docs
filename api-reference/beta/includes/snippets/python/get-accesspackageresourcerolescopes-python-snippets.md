---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = AccessPackageRequestBuilder.AccessPackageRequestBuilderGetQueryParameters(
		expand = ["accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)"],
)

request_configuration = AccessPackageRequestBuilder.AccessPackageRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.identityGovernance.entitlementManagement.accessPackages_by_id('accessPackage-id').get(request_configuration = request_configuration)


```