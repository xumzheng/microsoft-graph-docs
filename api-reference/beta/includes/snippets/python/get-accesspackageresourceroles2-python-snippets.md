---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = AccessPackageResourceRolesRequestBuilder.AccessPackageResourceRolesRequestBuilderGetQueryParameters(
		filter = "(originSystem eq 'SharePointOnline' and accessPackageResource/id eq '53c71803-a0a8-4777-aecc-075de8ee3991')",
		select = ["displayName","originId"],
)

request_configuration = AccessPackageResourceRolesRequestBuilder.AccessPackageResourceRolesRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.identityGovernance.entitlementManagement.accessPackageCatalogs_by_id('accessPackageCatalog-id').accessPackageResourceRoles.get(request_configuration = request_configuration)


```