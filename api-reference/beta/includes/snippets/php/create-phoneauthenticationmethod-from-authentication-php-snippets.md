---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PhoneAuthenticationMethod();


$requestRequestBody->setPhoneNumber('+1 2065555555');
$requestRequestBody->setPhoneType(new AuthenticationPhoneType('mobile'));
$result =  $graphClient->me()->authentication()->phoneMethods()->post($requestRequestBody);


```