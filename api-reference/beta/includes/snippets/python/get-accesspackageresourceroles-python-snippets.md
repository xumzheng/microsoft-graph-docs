---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = AccessPackageResourceRolesRequestBuilderGetRequestConfiguration(
request_configuration = AccessPackageResourceRolesRequestBuilderGetRequestConfiguration(query_params=query_params = AccessPackageResourceRolesRequestBuilderGetQueryParameters()
query_params['filter'] = "(originSystem eq 'AadGroup' and accessPackageResource/id eq 'a35bef72-a8aa-4ca3-af30-f6b2ece7208f')"
query_params['expand'] = ["accessPackageResource"]

)
query_params = AccessPackageResourceRolesRequestBuilderGetQueryParameters()
query_params['filter'] = "(originSystem eq 'AadGroup' and accessPackageResource/id eq 'a35bef72-a8aa-4ca3-af30-f6b2ece7208f')"
query_params['expand'] = ["accessPackageResource"]

)


result = await client.identityGovernance.entitlementManagement.accessPackageCatalogs_by_id('accessPackageCatalog-id').accessPackageResourceRoles.get(request_configuration)


```