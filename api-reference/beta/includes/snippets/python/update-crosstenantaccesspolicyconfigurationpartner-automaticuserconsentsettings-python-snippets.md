---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Cross_tenant_access_policy_configuration_partner()
automatic_user_consent_settings = Inbound_outbound_policy_configuration()
automatic_user_consent_settings.inbound_allowed = True

automatic_user_consent_settings.outbound_allowed = True


request_body.automatic_user_consent_settings = automatic_user_consent_settings



result = await client.policies.cro_tenant_acce_policy.partners.by_partner_id('crossTenantAccessPolicyConfigurationPartner-tenantId').patch(request_body = request_body)


```