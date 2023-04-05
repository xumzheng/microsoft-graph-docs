---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageCatalog()
request_body.setDisplayName('Catalog One')



result = await client.identityGovernance.entitlementManagement.catalogs._by_id('accessPackageCatalog-id').patch(request_body)


```