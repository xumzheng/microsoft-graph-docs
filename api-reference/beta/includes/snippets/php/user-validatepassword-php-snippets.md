---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PasswordRequestBody();


$requestRequestBody->setPassword('1234567890');
$result =  $graphClient->users()->validatePassword()->post($requestRequestBody);


```