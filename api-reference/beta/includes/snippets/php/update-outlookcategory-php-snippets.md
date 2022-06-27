---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OutlookCategory();


$requestRequestBody->setColor(new CategoryColor('preset15'));
$result =  $graphClient->me()->outlook()->masterCategoriesById('outlookCategory-id')->patch($requestRequestBody);


```