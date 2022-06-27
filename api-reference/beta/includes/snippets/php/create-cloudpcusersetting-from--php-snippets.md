---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CloudPcUserSetting();


$requestRequestBody->setDisplayName('Example');
$requestRequestBody->setSelfServiceEnabled(False);
$requestRequestBody->setLocalAdminEnabled(True);

$restorePointSetting = new CloudPcRestorePointSetting();
$requestRequestBody->setRestorePointSetting($restorePointSetting);


$restorePointSetting->setFrequencyInHours(16);
$restorePointSetting->setUserRestoreEnabled(True);

$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.cloudPcUserSetting',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->deviceManagement()->virtualEndpoint()->userSettings()->post($requestRequestBody);


```