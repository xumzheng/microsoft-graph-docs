---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = TenantTag();
requestBody.setDisplayName('Support');

requestBody.setDescription('Tenants that have purchased extended support');



requestResult = graphServiceClient.tenantRelationships().managedTenants().tenantTags().post(requestBody);


```