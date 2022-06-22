---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CloudPcProvisioningPolicy();


$requestRequestBody->setDescription('Description value');
$requestRequestBody->setDisplayName('Display Name value');

$domainJoinConfiguration = new CloudPcDomainJoinConfiguration();
$requestRequestBody->setDomainJoinConfiguration($domainJoinConfiguration);


$domainJoinConfiguration->setOnPremisesConnectionId('16ee6c71-fc10-438b-88ac-daa1ccafffff');
$domainJoinConfigurationAdditionalData = [
	"domainJoinType" => 'hybridAzureADJoin',
];
$domainJoinConfiguration->setAdditionalData($domainJoinConfigurationAdditionalData);

$requestRequestBody->setId('1d164206-bf41-4fd2-8424-a3192d39ffff');
$requestRequestBody->setImageDisplayName('Windows-10 19h1-evd');
$requestRequestBody->setImageId('MicrosoftWindowsDesktop_Windows-10_19h1-evd');
$requestRequestBody->setImageType(new CloudPcProvisioningPolicyImageType('gallery'));
$requestRequestBody->setOnPremisesConnectionId('4e47d0f6-6f77-44f0-8893-c0fe1701ffff');

$windowsSettings = new CloudPcWindowsSettings();
$requestRequestBody->setWindowsSettings($windowsSettings);


$windowsSettings->setLanguage('en-US');

$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.cloudPcProvisioningPolicy',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->deviceManagement()->virtualEndpoint()->provisioningPolicies()->post($requestRequestBody);


```