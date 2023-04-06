---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentitySynchronizationPutRequestBody()
additionalData = [
'displayName' => 'Fabrikam', 
'userSyncInbound' => request_body = UserSyncInbound()
		request_body.setIsSyncAllowed(true)


request_body.setUserSyncInbound($userSyncInbound)

];
request_body.setAdditionalData(additionalData)




await client.policies.crossTenantAccessPolicy.partners_by_id('crossTenantAccessPolicyConfigurationPartner-tenantId').identitySynchronization.put(request_body, headers=)


```