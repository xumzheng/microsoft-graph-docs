---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new B2xIdentityUserFlow();


$requestRequestBody->setId('Partner');
$requestRequestBody->setUserFlowType(new UserFlowType('signUpOrSignIn'));
$requestRequestBody->setUserFlowTypeVersion(1);
$identityProvidersArray = [];

$identityProviders1 = new IdentityProvider();

$identityProviders1->setId('Facebook-OAuth');
$identityProviders1->setType('Facebook');
$identityProviders1->setName('Facebook');

$identityProvidersArray []= $identityProviders1;
$requestRequestBody->setIdentityProviders($identityProvidersArray);
$result =  $graphClient->identity()->b2xUserFlows()->post($requestRequestBody);


```