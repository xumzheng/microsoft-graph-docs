---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AccessPackageRequestBuilderGetRequestConfiguration()

query_params = AccessPackageRequestBuilderGetQueryParameters()
query_params.expand = ["accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)"]

request_config.queryParameters = query_params


result = await client.identityGovernance.entitlementManagement.accessPackages._by_id('accessPackage-id').get(request_config)


```