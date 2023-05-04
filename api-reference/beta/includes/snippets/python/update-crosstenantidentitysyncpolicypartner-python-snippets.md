---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Cross_tenant_identity_sync_policy_partner()
user_sync_inbound = Cross_tenant_user_sync_inbound()
user_sync_inbound.is_sync_allowed = True


request_body.user_sync_inbound = user_sync_inbound



result = await client.policies.cro_tenant_acce_policy.partners.by_partner_id('crossTenantAccessPolicyConfigurationPartner-tenantId').identity_synchronization.patch(request_body = request_body)


```