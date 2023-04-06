---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CrossTenantAccessPolicyConfigurationPartner()
automaticUserConsentSettings = InboundOutboundPolicyConfiguration()
automaticUserConsentSettings.setInboundAllowed(true)

automaticUserConsentSettings.setOutboundAllowed(true)


request_body.setAutomaticUserConsentSettings($automaticUserConsentSettings)

request_config = CrossTenantAccessPolicyConfigurationPartnerRequestBuilderPatchRequestConfiguration(
request_config = CrossTenantAccessPolicyConfigurationPartnerRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.policies.crossTenantAccessPolicy.partners_by_id('crossTenantAccessPolicyConfigurationPartner-tenantId').patch(request_body, headers=)


```