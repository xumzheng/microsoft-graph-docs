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
$identityProvidersArray = [];

$identityProviders1 = new IdentityProvider();

$identityProviders1->setId('Facebook-OAuth');

$identityProvidersArray []= $identityProviders1;
$requestRequestBody->setIdentityProviders($identityProvidersArray);
$requestConfiguration = new B2cUserFlowsRequestBuilderPostRequestConfiguration();

$headers = [
"Location" => "https://graph.microsoft.com/beta/identity/b2cUserFlows('B2C_1_Customer')",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->identity()->b2cUserFlows()->post($requestRequestBody, $requestConfiguration);


```