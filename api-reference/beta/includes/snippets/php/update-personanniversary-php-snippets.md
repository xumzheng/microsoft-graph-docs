---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PersonAnnualEvent();


$requestRequestBody->setAllowedAudiences(new AllowedAudiences('contacts'));
$result =  $graphClient->me()->profile()->anniversariesById('personAnnualEvent-id')->patch($requestRequestBody);


```