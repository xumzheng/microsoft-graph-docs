---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OutlookCategory();


$requestRequestBody->setDisplayName('Project expenses');
$requestRequestBody->setColor(new CategoryColor('preset9'));
$result =  $graphClient->me()->outlook()->masterCategories()->post($requestRequestBody);


```