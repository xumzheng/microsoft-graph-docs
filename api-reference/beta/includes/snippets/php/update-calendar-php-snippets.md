---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Calendar();


$requestRequestBody->setName('Social events');
$result =  $graphClient->me()->calendar()->patch($requestRequestBody);


```