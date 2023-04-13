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
		request_body.is_sync_allowed = True


request_body.user_sync_inbound = userSyncInbound

];
request_body.additionaldata(additionalData)





await client.policies.crossTenantAccessPolicy.partners_by_id('crossTenantAccessPolicyConfigurationPartner-tenantId').identitySynchronization.put(request_body = request_body)


```