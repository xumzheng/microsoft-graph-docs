---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CloudPcDeviceImage();


$requestRequestBody->setDisplayName('Display Name value');
$requestRequestBody->setOsBuildNumber('OS Build Number value');
$requestRequestBody->setOperatingSystem('Operating System value');
$requestRequestBody->setVersion('Version value');
$requestRequestBody->setSourceImageResourceId('/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.cloudPcDeviceImage',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->deviceManagement()->virtualEndpoint()->deviceImages()->post($requestRequestBody);


```