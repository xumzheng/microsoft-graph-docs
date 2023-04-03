---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = TenantSearchPostRequestBody();
requestBody.setTenantId('String');



requestResult = graphServiceClient.tenantRelationships().managedTenants().tenantGroups().managedTenantsTenantSearch().post(requestBody);


```