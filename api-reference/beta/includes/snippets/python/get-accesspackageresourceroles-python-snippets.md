---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = AccessPackageResourceRolesRequestBuilderGetRequestConfiguration();

query_params = AccessPackageResourceRolesRequestBuilderGetQueryParameters;
query_params.filter = "(originSystem eq 'AadGroup' and accessPackageResource/id eq 'a35bef72-a8aa-4ca3-af30-f6b2ece7208f')";
query_params.expand = ["accessPackageResource"];

request_config.queryParameters = query_params;


result = await client.identityGovernance().entitlementManagement().accessPackageCatalogsById('accessPackageCatalog-id').accessPackageResourceRoles().get(request_config);


```