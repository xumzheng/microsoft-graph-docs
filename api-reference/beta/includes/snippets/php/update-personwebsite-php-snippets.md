---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PersonWebsite();


$requestRequestBody->setDescription('Lyn Damer play in the Women\'s 1st Division (Toppserien) in Norway');
$result =  $graphClient->me()->profile()->websitesById('personWebsite-id')->patch($requestRequestBody);


```