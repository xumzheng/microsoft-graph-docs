---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PersonAnnualEvent();


$requestRequestBody->setType(new PersonAnnualEventType('birthday'));
$requestRequestBody->setDate('1980-01-08');
$result =  $graphClient->me()->profile()->anniversaries()->post($requestRequestBody);


```