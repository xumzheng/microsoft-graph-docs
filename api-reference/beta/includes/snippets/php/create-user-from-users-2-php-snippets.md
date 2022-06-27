---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new User();


$requestRequestBody->setAccountEnabled(True);
$requestRequestBody->setDisplayName('Adele Vance');
$requestRequestBody->setMailNickname('AdeleV');
$requestRequestBody->setUserPrincipalName('AdeleV@contoso.onmicrosoft.com');

$passwordProfile = new PasswordProfile();
$requestRequestBody->setPasswordProfile($passwordProfile);


$passwordProfile->setForceChangePasswordNextSignIn(True);
$passwordProfile->setPassword('xWwvJ]6NMw+bWH-d');

$result =  $graphClient->users()->post($requestRequestBody);


```