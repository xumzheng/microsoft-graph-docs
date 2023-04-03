---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CrossTenantAccessPolicyConfigurationPartner();
automaticUserConsentSettings = InboundOutboundPolicyConfiguration();
automaticUserConsentSettings.setInboundAllowed(true);

automaticUserConsentSettings.setOutboundAllowed(true);


requestBody.setAutomaticUserConsentSettings($automaticUserConsentSettings);


result = await client.policies().crossTenantAccessPolicy().partnersById('crossTenantAccessPolicyConfigurationPartner-tenantId').patch(requestBody);


```