---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CrossTenantIdentitySyncPolicyPartner();
userSyncInbound = CrossTenantUserSyncInbound();
userSyncInbound.setIsSyncAllowed(true);


requestBody.setUserSyncInbound($userSyncInbound);


result = await client.policies().crossTenantAccessPolicy().partnersById('crossTenantAccessPolicyConfigurationPartner-tenantId').identitySynchronization().patch(requestBody);


```