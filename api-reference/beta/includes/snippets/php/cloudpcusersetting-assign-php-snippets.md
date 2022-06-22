---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AssignmentsRequestBody();


$assignmentsArray = [];

$assignments1 = new CloudPcUserSettingAssignment();

$assignments1AdditionalData = [
		"id" => 'b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff',
	];
$assignments1->setAdditionalData($assignments1AdditionalData);

$assignmentsArray []= $assignments1;
$requestRequestBody->setAssignments($assignmentsArray);
$result =  $graphClient->deviceManagement()->virtualEndpoint()->userSettingsById('cloudPcUserSetting-id')->assign()->post($requestRequestBody);


```