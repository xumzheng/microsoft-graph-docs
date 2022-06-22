---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new WebAccount();


$requestRequestBody->setWebUrl('https://github.com/innocenty.popov');
$result =  $graphClient->me()->profile()->webAccountsById('webAccount-id')->patch($requestRequestBody);


```