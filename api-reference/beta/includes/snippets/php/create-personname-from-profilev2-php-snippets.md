---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PersonName();


$requestRequestBody->setDisplayName('Innocenty Popov');
$requestRequestBody->setFirst('Innocenty');
$requestRequestBody->setInitials('IP');
$requestRequestBody->setLast('Popov');
$requestRequestBody->setLanguageTag('en-US');
$requestRequestBody->setMaiden(null);
$result =  $graphClient->me()->profile()->names()->post($requestRequestBody);


```