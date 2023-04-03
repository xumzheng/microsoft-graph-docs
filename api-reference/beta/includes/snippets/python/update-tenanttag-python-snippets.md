---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = TenantTag();
requestBody.setDisplayName('Onboarding');

requestBody.setDescription('Tenants that we are currently onboarding');



result = await client.tenantRelationships().managedTenants().tenantTagsById('tenantTag-id').patch(requestBody);


```