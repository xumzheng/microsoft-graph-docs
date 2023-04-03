---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = MoveToCatalogPostRequestBody();
requestBody.setCatalogId('3301434b-99bd-46be-923b-d762c30c8e8b');



graphServiceClient.identityGovernance().entitlementManagement().accessPackagesById('accessPackage-id').moveToCatalog().post(requestBody);


```