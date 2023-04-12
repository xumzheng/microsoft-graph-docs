---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageCatalog()
request_body.displayName = 'sales'

request_body.description = 'for employees working with sales and outside sales partners'

request_body.State(AccessPackageCatalogState('published'))

request_body.isExternallyVisible = true




result = await client.identityGovernance.entitlementManagement.catalogs.post(request_body = request_body)


```