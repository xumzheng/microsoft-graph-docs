---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AssignTagPostRequestBody();
requestBody.setTenantIds(['String', ]);



result = awaitclient.tenantRelationships().managedTenants().tenantTagsById('tenantTag-id').managedTenantsAssignTag().post(requestBody);


```