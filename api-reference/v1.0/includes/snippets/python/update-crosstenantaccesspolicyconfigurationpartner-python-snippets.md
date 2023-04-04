---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = CrossTenantAccessPolicyConfigurationPartner()
inboundTrust = CrossTenantAccessPolicyInboundTrust()
inboundTrust.setIsMfaAccepted(true)

inboundTrust.setIsCompliantDeviceAccepted(true)

inboundTrust.setIsHybridAzureADJoinedDeviceAccepted(true)


request_body.setInboundTrust($inboundTrust)


result = await client.policies.crossTenantAccessPolicy.partnersById('crossTenantAccessPolicyConfigurationPartner-tenantId').patch(request_body)


```