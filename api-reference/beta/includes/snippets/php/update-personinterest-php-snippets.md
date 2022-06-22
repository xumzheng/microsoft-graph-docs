---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PersonInterest();


$requestRequestBody->setCategories( [
'Sports',],
$result =  $graphClient->me()->profile()->interestsById('personInterest-id')->patch($requestRequestBody);


```