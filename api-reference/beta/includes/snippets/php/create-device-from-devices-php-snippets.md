---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Device();


$requestRequestBody->setAccountEnabled(True);
$alternativeSecurityIdsArray = [];

$alternativeSecurityIds1 = new AlternativeSecurityId();

$alternativeSecurityIds1AdditionalData = [
		"type" => 99,
		"identityProvider" => 'identityProvider-value',
		"key" => 'base64Y3YxN2E1MWFlYw==',
	];
$alternativeSecurityIds1->setAdditionalData($alternativeSecurityIds1AdditionalData);

$alternativeSecurityIdsArray []= $alternativeSecurityIds1;
$requestRequestBody->setAlternativeSecurityIds($alternativeSecurityIdsArray);
$requestRequestBody->setApproximateLastSignInDateTime(new DateTime("2016-10-19T10:37:00Z"));
$requestRequestBody->setDeviceId('deviceId-value');
$requestRequestBody->setDeviceMetadata('deviceMetadata-value');
$requestRequestBody->setDeviceVersion(99);
$result =  $graphClient->devices()->post($requestRequestBody);


```