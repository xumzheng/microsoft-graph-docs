---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AccessPackageCatalog();
requestBody.setDisplayName('Catalog One');



result = awaitclient.identityGovernance().entitlementManagement().catalogsById('accessPackageCatalog-id').patch(requestBody);


```