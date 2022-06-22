---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ItemEmail();


$requestRequestBody->setAddress('Innocenty.Popov@adventureworks.com');
$result =  $graphClient->me()->profile()->emails()->post($requestRequestBody);


```