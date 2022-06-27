---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new User();



$passwordProfile = new PasswordProfile();
$requestRequestBody->setPasswordProfile($passwordProfile);


$passwordProfile->setForceChangePasswordNextSignIn(False);
$passwordProfile->setPassword('xWwvJ]6NMw+bWH-d');

$result =  $graphClient->usersById('user-id')->patch($requestRequestBody);


```