---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageCatalog()
request_body.setDisplayName('Catalog One')


request_config = AccessPackageCatalogRequestBuilderPatchRequestConfiguration(
request_config = AccessPackageCatalogRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.identityGovernance.entitlementManagement.accessPackageCatalogs_by_id('accessPackageCatalog-id').patch(request_body, headers=)


```