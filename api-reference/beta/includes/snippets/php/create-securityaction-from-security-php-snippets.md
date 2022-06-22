---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SecurityAction();


$requestRequestBody->setName('BlockIp');
$requestRequestBody->setActionReason('Test');
$parametersArray = [];

$parameters1 = new KeyValuePair();

$parameters1->setName('IP');
$parameters1->setValue('1.2.3.4');

$parametersArray []= $parameters1;
$requestRequestBody->setParameters($parametersArray);

$vendorInformation = new SecurityVendorInformation();
$requestRequestBody->setVendorInformation($vendorInformation);


$vendorInformation->setProvider('Windows Defender ATP');
$vendorInformation->setVendor('Microsoft');

$result =  $graphClient->security()->securityActions()->post($requestRequestBody);


```