---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CrossTenantAccessPolicyConfigurationPartner();
$inboundTrust = new CrossTenantAccessPolicyInboundTrust();
$inboundTrust->setIsMfaAccepted(true);

$inboundTrust->setIsCompliantDeviceAccepted(true);

$inboundTrust->setIsHybridAzureADJoinedDeviceAccepted(true);


$requestBody->setInboundTrust($inboundTrust);


$requestResult = $graphServiceClient->policies()->crossTenantAccessPolicy()->partnersById('crossTenantAccessPolicyConfigurationPartner-tenantId')->patch($requestBody);


```