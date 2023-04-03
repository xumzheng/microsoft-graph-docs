---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AccessPackage();
requestBody.setDisplayName('Access Package New Name');



result = awaitclient.identityGovernance().entitlementManagement().accessPackagesById('accessPackage-id').patch(requestBody);


```