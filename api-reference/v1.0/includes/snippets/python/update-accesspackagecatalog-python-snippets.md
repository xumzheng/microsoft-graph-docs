---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AccessPackageCatalog();
requestBody.setDisplayName('Catalog One');



result = await client.identityGovernance().entitlementManagement().catalogsById('accessPackageCatalog-id').patch(requestBody);


```