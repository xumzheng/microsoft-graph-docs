---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageCatalog()
request_body.setDisplayName('sales')

request_body.setDescription('for employees working with sales and outside sales partners')

request_body.setIsExternallyVisible(true)



result = await client.identityGovernance_entitlementManagement_accessPackageCatalogs.post(request_body)


```