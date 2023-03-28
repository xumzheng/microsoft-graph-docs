---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new SecurityAction();
$requestBody->setName('BlockIp');

$requestBody->setActionReason('Test');

$parametersKeyValuePair1 = new KeyValuePair();
$parametersKeyValuePair1->setName('IP');

$parametersKeyValuePair1->setValue('1.2.3.4');


$parametersArray []= $parametersKeyValuePair1;
$requestBody->setParameters($parametersArray);


$vendorInformation = new SecurityVendorInformation();
$vendorInformation->setProvider('Windows Defender ATP');

$vendorInformation->setVendor('Microsoft');


$requestBody->setVendorInformation($vendorInformation);


$requestResult = $graphServiceClient->security()->securityActions()->post($requestBody);


```