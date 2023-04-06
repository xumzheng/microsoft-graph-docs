---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AccessPackageResourceRolesRequestBuilderGetRequestConfiguration(
request_config = AccessPackageResourceRolesRequestBuilderGetRequestConfiguration(query_params=query_params = AccessPackageResourceRolesRequestBuilderGetQueryParameters()
query_params.filter = "(originSystem eq 'AadGroup' and accessPackageResource/id eq '4a1e21c5-8a76-4578-acb1-641160e076e8' and displayName eq 'Member')"
query_params.expand = ["accessPackageResource"]

)
query_params = AccessPackageResourceRolesRequestBuilderGetQueryParameters()
query_params.filter = "(originSystem eq 'AadGroup' and accessPackageResource/id eq '4a1e21c5-8a76-4578-acb1-641160e076e8' and displayName eq 'Member')"
query_params.expand = ["accessPackageResource"]

)


result = await client.identityGovernance.entitlementManagement.accessPackageCatalogs_by_id('accessPackageCatalog-id').accessPackageResourceRoles.get(request_config, headers=request_config)


```