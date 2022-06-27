---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UserAccountInformation();


$requestRequestBody->setCountryCode('NO');
$result =  $graphClient->me()->profile()->accountById('userAccountInformation-id')->patch($requestRequestBody);


```