---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Notebook();


$requestRequestBody->setDisplayName('My Private notebook');
$result =  $graphClient->me()->onenote()->notebooks()->post($requestRequestBody);


```