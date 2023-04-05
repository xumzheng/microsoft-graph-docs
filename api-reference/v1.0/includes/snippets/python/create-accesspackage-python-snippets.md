---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackage()
request_body.setDisplayName('sales reps')

request_body.setDescription('outside sales representatives')

request_body.setIsHidden(false)

catalog = AccessPackageCatalog()
catalog.setId('66584aae-98bb-48cc-9458-7bee5d2a6577')


request_body.setCatalog($catalog)


result = await client.identityGovernance.entitlementManagement.accessPackages.post(request_body)


```