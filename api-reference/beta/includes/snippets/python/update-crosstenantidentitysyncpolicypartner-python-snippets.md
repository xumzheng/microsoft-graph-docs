---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CrossTenantIdentitySyncPolicyPartner()
userSyncInbound = CrossTenantUserSyncInbound()
userSyncInbound.setIsSyncAllowed(true)


request_body.setUserSyncInbound($userSyncInbound)


result = await client.policies.crossTenantAccessPolicy.partners_by_id('crossTenantAccessPolicyConfigurationPartner-tenantId').identitySynchronization.patch(request_body, headers=)


```