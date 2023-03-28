---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PhoneAuthenticationMethod();
$requestBody->setPhoneNumber('+1 2065555554');

$requestBody->setPhoneType(new AuthenticationPhoneType('mobile'));



$requestResult = $graphServiceClient->me()->authentication()->phoneMethodsById('phoneAuthenticationMethod-id')->patch($requestBody);


```