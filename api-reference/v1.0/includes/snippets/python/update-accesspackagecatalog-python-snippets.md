---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AccessPackageCatalog();
requestBody.setDisplayName('Catalog One');



requestResult = graphServiceClient.identityGovernance().entitlementManagement().catalogsById('accessPackageCatalog-id').patch(requestBody);


```