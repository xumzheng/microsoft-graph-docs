---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TemporaryAccessPassAuthenticationMethod();


$requestRequestBody->setStartDateTime(new DateTime("2022-06-05T00:00:00.000Z"));
$requestRequestBody->setLifetimeInMinutes(60);
$requestRequestBody->setIsUsableOnce(False);
$result =  $graphClient->usersById('user-id')->authentication()->temporaryAccessPassMethods()->post($requestRequestBody);


```