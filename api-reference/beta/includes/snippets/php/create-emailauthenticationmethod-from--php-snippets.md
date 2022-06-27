---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EmailAuthenticationMethod();


$requestRequestBody->setEmailAddress('kim@contoso.com');
$result =  $graphClient->usersById('user-id')->authentication()->emailMethods()->post($requestRequestBody);


```