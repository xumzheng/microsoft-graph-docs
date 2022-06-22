---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Device();



$extensionAttributes = new OnPremisesExtensionAttributes();
$requestRequestBody->setExtensionAttributes($extensionAttributes);


$extensionAttributes->setExtensionAttribute1('BYOD-Device');

$result =  $graphClient->devicesById('device-id')->patch($requestRequestBody);


```