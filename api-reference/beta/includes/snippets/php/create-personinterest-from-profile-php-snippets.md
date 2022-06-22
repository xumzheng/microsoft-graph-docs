---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PersonInterest();


$requestRequestBody->setCategories( [
'Sports',],
$requestRequestBody->setDescription('World\'s greatest football club');
$requestRequestBody->setDisplayName('Chelsea FC');
$requestRequestBody->setWebUrl('https://www.chelseafc.com');
$result =  $graphClient->me()->profile()->interests()->post($requestRequestBody);


```