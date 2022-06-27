---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CloudPcProvisioningPolicy();


$requestRequestBody->setDisplayName('HR provisioning policy');
$requestRequestBody->setDescription('Provisioning policy for India HR employees');
$requestRequestBody->setOnPremisesConnectionId('4e47d0f6-6f77-44f0-8893-c0fe1701ffff');
$requestRequestBody->setImageId('Image ID value');
$requestRequestBody->setImageDisplayName('Image Display Name value');
$requestRequestBody->setImageType(new CloudPcProvisioningPolicyImageType('custom'));

$windowsSettings = new CloudPcWindowsSettings();
$requestRequestBody->setWindowsSettings($windowsSettings);


$windowsSettings->setLanguage('en-US');

$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.cloudPcProvisioningPolicy',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->deviceManagement()->virtualEndpoint()->provisioningPoliciesById('cloudPcProvisioningPolicy-id')->patch($requestRequestBody);


```