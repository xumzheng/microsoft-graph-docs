---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CrossTenantAccessPolicyConfigurationPartner();
$automaticUserConsentSettings = new InboundOutboundPolicyConfiguration();
$automaticUserConsentSettings.setInboundAllowed(true);

$automaticUserConsentSettings.setOutboundAllowed(true);


$requestBody.setAutomaticUserConsentSettings($automaticUserConsentSettings);


$requestResult = $graphServiceClient.policies().crossTenantAccessPolicy().partnersById('crossTenantAccessPolicyConfigurationPartner-tenantId').patch($requestBody);


```