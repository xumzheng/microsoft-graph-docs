---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CrossTenantIdentitySyncPolicyPartner();
$userSyncInbound = new CrossTenantUserSyncInbound();
$userSyncInbound->setIsSyncAllowed(true);


$requestBody->setUserSyncInbound($userSyncInbound);


$requestResult = $graphServiceClient->policies()->crossTenantAccessPolicy()->partnersById('crossTenantAccessPolicyConfigurationPartner-tenantId')->identitySynchronization()->patch($requestBody);


```