---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Subscription();


$requestRequestBody->setExpirationDateTime(new DateTime("2016-11-22T18:23:45.9356913Z"));
$result =  $graphClient->subscriptionsById('subscription-id')->patch($requestRequestBody);


```