---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AuthenticationFlowsPolicy();



$selfServiceSignUp = new SelfServiceSignUpAuthenticationFlowConfiguration();
$requestRequestBody->setSelfServiceSignUp($selfServiceSignUp);


$selfServiceSignUp->setIsEnabled(True);

$result =  $graphClient->policies()->authenticationFlowsPolicy()->patch($requestRequestBody);


```