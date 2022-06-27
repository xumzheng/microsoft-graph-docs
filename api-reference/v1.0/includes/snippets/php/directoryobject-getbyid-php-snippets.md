---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new GetByIdsPostRequestBody();


$requestRequestBody->setIds(['84b80893874940a3-97b7-68513b600544','5d6059b6368d-45f8-91e18e07d485f1d0',]);
$requestRequestBody->setTypes(['user',]);
$result =  $graphClient->directoryObjects()->getByIds()->post($requestRequestBody);


```