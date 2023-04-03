---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = UnassignTagPostRequestBody();
requestBody.setTenantIds(['String', ]);



requestResult = graphServiceClient.tenantRelationships().managedTenants().tenantTagsById('tenantTag-id').managedTenantsUnassignTag().post(requestBody);


```