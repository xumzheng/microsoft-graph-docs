---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new B2cAuthenticationMethodsPolicy();
$requestBody->setIsEmailPasswordAuthenticationEnabled(false);

$requestBody->setIsUserNameAuthenticationEnabled(true);

$requestBody->setIsPhoneOneTimePasswordAuthenticationEnabled(true);



$requestResult = $graphServiceClient->policies()->b2cAuthenticationMethodsPolicy()->patch($requestBody);


```