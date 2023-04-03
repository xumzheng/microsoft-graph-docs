---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AccessPackage();
requestBody.setDisplayName('Access Package New Name');



result = await client.identityGovernance().entitlementManagement().accessPackagesById('accessPackage-id').patch(requestBody);


```