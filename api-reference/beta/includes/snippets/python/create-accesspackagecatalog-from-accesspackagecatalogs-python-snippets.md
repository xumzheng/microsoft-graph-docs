---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AccessPackageCatalog();
requestBody.setDisplayName('sales');

requestBody.setDescription('for employees working with sales and outside sales partners');

requestBody.setIsExternallyVisible(true);



result = awaitclient.identityGovernance().entitlementManagement().accessPackageCatalogs().post(requestBody);


```