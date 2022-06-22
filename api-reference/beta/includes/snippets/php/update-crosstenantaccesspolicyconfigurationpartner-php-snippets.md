---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CrossTenantAccessPolicyConfigurationPartner();



$inboundTrust = new CrossTenantAccessPolicyInboundTrust();
$requestRequestBody->setInboundTrust($inboundTrust);


$inboundTrust->setIsMfaAccepted(True);
$inboundTrust->setIsCompliantDeviceAccepted(True);
$inboundTrust->setIsHybridAzureADJoinedDeviceAccepted(True);

$result =  $graphClient->policies()->crossTenantAccessPolicy()->partnersById('crossTenantAccessPolicyConfigurationPartner-tenantId')->patch($requestRequestBody);


```