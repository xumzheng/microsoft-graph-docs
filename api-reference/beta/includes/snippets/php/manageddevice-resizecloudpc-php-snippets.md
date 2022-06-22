---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TargetServicePlanIdRequestBody();


$requestRequestBody->setTargetServicePlanId('30d0e128-de93-41dc-89ec-33d84bb662a0');
$result =  $graphClient->deviceManagement()->managedDevicesById('managedDevice-id')->resizeCloudPc()->post($requestRequestBody);


```