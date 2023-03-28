---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CloudPcProvisioningPolicy();
$requestBody->set@odatatype('#microsoft.graph.cloudPcProvisioningPolicy');

$requestBody->setDescription('Description value');

$requestBody->setDisplayName('Display Name value');

$domainJoinConfiguration = new CloudPcDomainJoinConfiguration();
$domainJoinConfiguration->setOnPremisesConnectionId('16ee6c71-fc10-438b-88ac-daa1ccafffff');

$additionalData = [
'domainJoinType' => 'hybridAzureADJoin', 
];
$domainJoinConfiguration->setAdditionalData($additionalData);



$requestBody->setDomainJoinConfiguration($domainJoinConfiguration);
$requestBody->setEnableSingleSignOn(true);

$requestBody->setImageDisplayName('Windows-10 19h1-evd');

$requestBody->setImageId('MicrosoftWindowsDesktop_Windows-10_19h1-evd');

$requestBody->setImageType(new CloudPcProvisioningPolicyImageType('gallery'));

$requestBody->setOnPremisesConnectionId('4e47d0f6-6f77-44f0-8893-c0fe1701ffff');

$windowsSettings = new CloudPcWindowsSettings();
$windowsSettings->setLanguage('en-US');


$requestBody->setWindowsSettings($windowsSettings);
$requestBody->setProvisioningType(new CloudPcProvisioningType('dedicated'));



$requestResult = $graphServiceClient->deviceManagement()->virtualEndpoint()->provisioningPolicies()->post($requestBody);


```