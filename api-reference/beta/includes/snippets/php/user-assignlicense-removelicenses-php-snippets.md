---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AssignLicensePostRequestBody();


$addLicensesArray = [];
$requestRequestBody->setAddLicenses($addLicensesArray);
$requestRequestBody->setRemoveLicenses(['f30db892-07e9-47e9-837c-80727f46fd3d','84a661c4-e949-4bd2-a560-ed7766fcaf2b',]);
$result =  $graphClient->me()->assignLicense()->post($requestRequestBody);


```