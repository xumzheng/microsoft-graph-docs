---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PersonWebsite();


$requestRequestBody->setCategories( [
'football',],
$requestRequestBody->setDisplayName('Lyn Damer');
$requestRequestBody->setWebUrl('www.lyndamer.no');
$result =  $graphClient->me()->profile()->websites()->post($requestRequestBody);


```