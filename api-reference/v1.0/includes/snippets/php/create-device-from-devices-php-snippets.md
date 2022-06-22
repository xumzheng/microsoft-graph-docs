---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Device();


$requestRequestBody->setAccountEnabled(False);
$alternativeSecurityIdsArray = [];

$alternativeSecurityIds1 = new AlternativeSecurityId();

$alternativeSecurityIds1AdditionalData = [
		"type" => 2,
		"key" => 'base64Y3YxN2E1MWFlYw==',
	];
$alternativeSecurityIds1->setAdditionalData($alternativeSecurityIds1AdditionalData);

$alternativeSecurityIdsArray []= $alternativeSecurityIds1;
$requestRequestBody->setAlternativeSecurityIds($alternativeSecurityIdsArray);
$requestRequestBody->setDeviceId('4c299165-6e8f-4b45-a5ba-c5d250a707ff');
$requestRequestBody->setDisplayName('Test device');
$requestRequestBody->setOperatingSystem('linux');
$requestRequestBody->setOperatingSystemVersion('1');
$result =  $graphClient->devices()->post($requestRequestBody);


```