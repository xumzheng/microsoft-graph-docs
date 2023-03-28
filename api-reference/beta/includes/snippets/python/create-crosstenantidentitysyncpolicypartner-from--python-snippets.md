---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new IdentitySynchronizationPutRequestBody();
$additionalData = [
'displayName' => 'Fabrikam', 
'userSyncInbound' => $requestBody = new UserSyncInbound();
		$requestBody->setIsSyncAllowed(true);


$requestBody->setUserSyncInbound($userSyncInbound);

];
$requestBody->setAdditionalData($additionalData);




$graphServiceClient->policies()->crossTenantAccessPolicy()->partnersById('crossTenantAccessPolicyConfigurationPartner-tenantId')->identitySynchronization()->put($requestBody);


```