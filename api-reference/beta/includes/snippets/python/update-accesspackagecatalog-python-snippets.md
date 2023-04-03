---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AccessPackageCatalog();
requestBody.setDisplayName('Catalog One');



result = await client.identityGovernance().entitlementManagement().accessPackageCatalogsById('accessPackageCatalog-id').patch(requestBody);


```