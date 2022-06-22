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
'113feb6c-3fe4-4440-bddc-54d774bf0318','14ab5db5-e6c4-4b20-b4bc-13e36fd2227f',		],
		"skuId" => 'b05e124f-c7cc-45a0-a6aa-8cf78c946968',
	];
$addLicenses1->setAdditionalData($addLicenses1AdditionalData);

$addLicensesArray []= $addLicenses1;

$addLicenses2 = new AssignedLicense();

$addLicenses2AdditionalData = [
	"disabledPlans" =>  [
'a413a9ff-720c-4822-98ef-2f37c2a21f4c',	],
	"skuId" => 'c7df2760-2c81-4ef7-b578-5b5392b571df',
];
$addLicenses2->setAdditionalData($addLicenses2AdditionalData);

$addLicensesArray []= $addLicenses2;
$requestRequestBody->setAddLicenses($addLicensesArray);
$requestRequestBody->setRemoveLicenses( [
],
$result =  $graphClient->groupsById('group-id')->assignLicense()->post($requestRequestBody);


```