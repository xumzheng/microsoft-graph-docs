---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CrossTenantAccessPolicyConfigurationPartner();
inboundTrust = CrossTenantAccessPolicyInboundTrust();
inboundTrust.setIsMfaAccepted(true);

inboundTrust.setIsCompliantDeviceAccepted(true);

inboundTrust.setIsHybridAzureADJoinedDeviceAccepted(true);


requestBody.setInboundTrust($inboundTrust);


result = await client.policies().crossTenantAccessPolicy().partnersById('crossTenantAccessPolicyConfigurationPartner-tenantId').patch(requestBody);


```