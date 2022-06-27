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
	"disabledPlans" => ['8a256a2b-b617-496d-b51b-e76466e88db0',],
"skuId" => '84a661c4-e949-4bd2-a560-ed7766fcaf2b',
];
$addLicensesaddLicenses1->setAdditionalData($addLicensesaddLicenses1AdditionalData);

$addLicensesArray []= $addLicensesaddLicenses1;

$addLicensesaddLicenses2 = new AssignedLicense();

$addLicensesaddLicenses2AdditionalData = [
"disabledPlans" => [],
"skuId" => 'f30db892-07e9-47e9-837c-80727f46fd3d',
];
$addLicensesaddLicenses2->setAdditionalData($addLicensesaddLicenses2AdditionalData);

$addLicensesArray []= $addLicensesaddLicenses2;
$requestRequestBody->setAddLicenses($addLicensesArray);
$requestRequestBody->setRemoveLicenses([]);
$result =  $graphClient->me()->assignLicense()->post($requestRequestBody);


```