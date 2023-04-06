---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackage()
request_body.setDisplayName('Access Package New Name')



result = await client.identityGovernance.entitlementManagement.accessPackages_by_id('accessPackage-id').patch(request_body)


```