---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CrossTenantAccessPolicyConfigurationPartner()
inbound_trust = CrossTenantAccessPolicyInboundTrust()
inboundTrust.is_mfa_accepted = True

inboundTrust.is_compliant_device_accepted = True

inboundTrust.is_hybrid_azure_a_d_joined_device_accepted = True


request_body.inbound_trust = inboundTrust



result = await client.policies.crossTenantAccessPolicy.partners_by_id('crossTenantAccessPolicyConfigurationPartner-tenantId').patch(request_body = request_body)


```