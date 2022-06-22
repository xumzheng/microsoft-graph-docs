---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AssignLicensePostRequestBody();


$addLicensesArray = [];
$requestRequestBody->setAddLicenses($addLicensesArray);
$requestRequestBody->setRemoveLicenses( [
'c7df2760-2c81-4ef7-b578-5b5392b571df','b05e124f-c7cc-45a0-a6aa-8cf78c946968',],
$result =  $graphClient->groupsById('group-id')->assignLicense()->post($requestRequestBody);


```