---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new WorkPosition();


$requestRequestBody->setIsCurrent(True);
$result =  $graphClient->me()->profile()->positionsById('workPosition-id')->patch($requestRequestBody);


```