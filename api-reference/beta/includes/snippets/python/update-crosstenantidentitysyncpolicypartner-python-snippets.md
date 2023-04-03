---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = CrossTenantIdentitySyncPolicyPartner();
userSyncInbound = CrossTenantUserSyncInbound();
userSyncInbound.setIsSyncAllowed(true);


requestBody.setUserSyncInbound($userSyncInbound);


requestResult = graphServiceClient.policies().crossTenantAccessPolicy().partnersById('crossTenantAccessPolicyConfigurationPartner-tenantId').identitySynchronization().patch(requestBody);


```