---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = AccessPackageResourceRolesRequestBuilderGetRequestConfiguration();

query_params = AccessPackageResourceRolesRequestBuilderGetQueryParameters();
query_params.filter = "(originSystem eq 'SharePointOnline' and accessPackageResource/id eq '53c71803-a0a8-4777-aecc-075de8ee3991')";
query_params.select = ["displayName","originId"];

request_config.queryParameters = query_params;


result = await client.identityGovernance().entitlementManagement().accessPackageCatalogsById('accessPackageCatalog-id').accessPackageResourceRoles().get(request_config);


```