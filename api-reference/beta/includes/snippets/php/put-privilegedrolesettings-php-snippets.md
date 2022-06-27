---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SettingsPutRequestBody();


$requestRequestBodyAdditionalData = [
	"id" => '9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3',
	"elevationDuration" => 'PT8H',
	"notificationToUserOnElevation" => False,
	"ticketingInfoOnElevation" => True,
	"mfaOnElevation" => False,
	"maxElavationDuration" => 'PT0S',
	"minElevationDuration" => 'PT0S',
	"lastGlobalAdmin" => False,
	"isMfaOnElevationConfigurable" => True,
	"approvalOnElevation" => False,
	"approverIds" => ['e2b2a2fb-13d7-495c-adc9-941fe966793f','22770e3f-b9b4-418e-9dea-d0e3d2f275dd',],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->privilegedRolesById('privilegedRole-id')->settings()->put($requestRequestBody);


```