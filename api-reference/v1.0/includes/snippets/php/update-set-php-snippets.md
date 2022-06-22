---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Set();


$requestRequestBody->setDescription('mySet');
$result =  $graphClient->sitesById('site-id')->termStore()->setsById('set-id')->patch($requestRequestBody);


```