---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackage()
request_body.setCatalogId('cec5d6ab-c75d-47c0-9c1c-92e89f66e384')

request_body.setDisplayName('Marketing Campaign')

request_body.setDescription('Access to resources for the campaign')



result = await client.identityGovernance.entitlementManagement.accessPackages.post(request_body, headers=)


```