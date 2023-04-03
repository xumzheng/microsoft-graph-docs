---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = CrossTenantAccessPolicyConfigurationPartner();
automaticUserConsentSettings = InboundOutboundPolicyConfiguration();
automaticUserConsentSettings.setInboundAllowed(true);

automaticUserConsentSettings.setOutboundAllowed(true);


requestBody.setAutomaticUserConsentSettings($automaticUserConsentSettings);


result = awaitclient.policies().crossTenantAccessPolicy().partnersById('crossTenantAccessPolicyConfigurationPartner-tenantId').patch(requestBody);


```