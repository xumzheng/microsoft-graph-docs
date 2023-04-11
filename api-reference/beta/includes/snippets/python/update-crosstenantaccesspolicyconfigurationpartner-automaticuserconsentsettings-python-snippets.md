---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CrossTenantAccessPolicyConfigurationPartner()
automaticUserConsentSettings = InboundOutboundPolicyConfiguration()
automaticUserConsentSettings.inboundAllowed = true

automaticUserConsentSettings.outboundAllowed = true


request_body.automaticUserConsentSettings = automaticUserConsentSettings


request_configuration = CrossTenantAccessPolicyConfigurationPartnerRequestBuilderPatchRequestConfiguration(
)


result = await client.policies.crossTenantAccessPolicy.partners_by_id('crossTenantAccessPolicyConfigurationPartner-tenantId').patch(request_body = request_body)


```