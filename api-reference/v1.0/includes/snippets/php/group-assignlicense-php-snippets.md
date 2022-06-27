---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AssignLicensePostRequestBody();


$addLicensesArray = [];

$addLicensesaddLicenses1 = new AssignedLicense();

$addLicensesaddLicenses1AdditionalData = [
	"disabledPlans" => ['113feb6c-3fe4-4440-bddc-54d774bf0318','14ab5db5-e6c4-4b20-b4bc-13e36fd2227f',],
"skuId" => 'b05e124f-c7cc-45a0-a6aa-8cf78c946968',
];
$addLicensesaddLicenses1->setAdditionalData($addLicensesaddLicenses1AdditionalData);

$addLicensesArray []= $addLicensesaddLicenses1;

$addLicensesaddLicenses2 = new AssignedLicense();

$addLicensesaddLicenses2AdditionalData = [
"disabledPlans" => ['a413a9ff-720c-4822-98ef-2f37c2a21f4c',],
"skuId" => 'c7df2760-2c81-4ef7-b578-5b5392b571df',
];
$addLicensesaddLicenses2->setAdditionalData($addLicensesaddLicenses2AdditionalData);

$addLicensesArray []= $addLicensesaddLicenses2;
$requestRequestBody->setAddLicenses($addLicensesArray);
$requestRequestBody->setRemoveLicenses([]);
$result =  $graphClient->groupsById('group-id')->assignLicense()->post($requestRequestBody);


```