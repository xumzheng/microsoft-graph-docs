---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Application();
$additionalData = [
'onPremisesPublishing' => $requestBody = new OnPremisesPublishing();
$singleSignOnSettings = new SingleSignOnSettings();
$singleSignOnSettingsKerberosSignOnSettings = new KerberosSignOnSettings();
$		singleSignOnSettingsKerberosSignOnSettings->setKerberosServicePrincipalName('HTTP/iwademo.contoso.com');

$		singleSignOnSettingsKerberosSignOnSettings->setKerberosSignOnMappingAttributeType('userPrincipalName');


$singleSignOnSettings->setKerberosSignOnSettings($singleSignOnSettingsKerberosSignOnSettings);
$		singleSignOnSettings->setSingleSignOnMode('onPremisesKerberos');


$requestBody->setSingleSignOnSettings($singleSignOnSettings);

$requestBody->setOnPremisesPublishing($onPremisesPublishing);

];
$requestBody->setAdditionalData($additionalData);




$graphServiceClient->applicationsById('application-id')->patch($requestBody);


```