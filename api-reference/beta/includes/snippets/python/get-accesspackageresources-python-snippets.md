---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = AccessPackageResourcesRequestBuilderGetRequestConfiguration()

query_params = AccessPackageResourcesRequestBuilderGetQueryParameters()
query_params.filter = "resourceType eq 'Application'"
query_params.expand = ["accessPackageResourceScopes"]

request_config.queryParameters = query_params


result = await client.identityGovernance.entitlementManagement.accessPackageCatalogsById('accessPackageCatalog-id').accessPackageResources.get(request_config)


```