---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AssignLicensePostRequestBody();


$addLicensesArray = [];

$addLicenses1 = new AssignedLicense();

$addLicenses1AdditionalData = [
		"disabledPlans" =>  [
'11b0131d-43c8-4bbb-b2c8-e80f9a50834a',		],
		"skuId" => '45715bb8-13f9-4bf6-927f-ef96c102d394',
	];
$addLicenses1->setAdditionalData($addLicenses1AdditionalData);

$addLicensesArray []= $addLicenses1;
$requestRequestBody->setAddLicenses($addLicensesArray);
$requestRequestBody->setRemoveLicenses( [
'bea13e0c-3828-4daa-a392-28af7ff61a0f',],
$result =  $graphClient->me()->assignLicense()->post($requestRequestBody);


```