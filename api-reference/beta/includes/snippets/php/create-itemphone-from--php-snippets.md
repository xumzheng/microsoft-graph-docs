---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ItemPhone();


$requestRequestBody->setDisplayName('Car Phone');
$requestRequestBody->setNumber('+7 499 342 22 13');
$result =  $graphClient->me()->profile()->phones()->post($requestRequestBody);


```