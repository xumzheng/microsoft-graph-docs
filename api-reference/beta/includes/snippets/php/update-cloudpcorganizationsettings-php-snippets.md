---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CloudPcOrganizationSettings();


$requestRequestBody->setUserAccountType(new CloudPcUserAccountType('standardUser'));
$requestRequestBody->setOsVersion(new CloudPcOperatingSystem('windows11'));

$windowsSettings = new CloudPcWindowsSettings();
$requestRequestBody->setWindowsSettings($windowsSettings);


$windowsSettings->setLanguage('en-US');

$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.cloudPcOrganizationSettings',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->deviceManagement()->virtualEndpoint()->organizationSettings()->patch($requestRequestBody);


```