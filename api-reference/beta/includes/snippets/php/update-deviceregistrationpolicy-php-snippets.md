---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DeviceRegistrationPolicyPutRequestBody();


$requestRequestBodyAdditionalData = [
	"id" => 'deviceRegistrationPolicy',
	"displayName" => 'Device Registration Policy',
	"description" => 'Tenant-wide policy that manages intial provisioning controls using quota restrictions, additional authentication and authorization checks',
	"userDeviceQuota" => 50,
	"multiFactorAuthConfiguration" => '0',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->deviceRegistrationPolicy()->put($requestRequestBody);


```