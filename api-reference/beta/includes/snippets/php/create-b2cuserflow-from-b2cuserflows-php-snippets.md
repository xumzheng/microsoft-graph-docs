---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new B2cIdentityUserFlow();


$requestRequestBody->setId('Customer');
$requestRequestBody->setUserFlowType(new UserFlowType('signUpOrSignIn'));
$requestRequestBody->setUserFlowTypeVersion(3);
$result =  $graphClient->identity()->b2cUserFlows()->post($requestRequestBody);


```