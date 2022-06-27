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

$identityProvidersidentityProviders1 = new IdentityProvider();

$identityProvidersidentityProviders1->setId('Facebook-OAuth');
$identityProvidersidentityProviders1->setType('Facebook');
$identityProvidersidentityProviders1->setName('Facebook');

$identityProvidersArray []= $identityProvidersidentityProviders1;
$requestRequestBody->setIdentityProviders($identityProvidersArray);
$result =  $graphClient->identity()->b2xUserFlows()->post($requestRequestBody);


```