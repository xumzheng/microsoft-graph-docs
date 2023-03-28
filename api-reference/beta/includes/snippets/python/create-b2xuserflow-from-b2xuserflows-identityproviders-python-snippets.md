---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new B2xIdentityUserFlow();
$requestBody->setId('Partner');

$requestBody->setUserFlowType(new UserFlowType('signuporsignin'));

$requestBody->setUserFlowTypeVersion(1);

$identityProvidersIdentityProvider1 = new IdentityProvider();
$identityProvidersIdentityProvider1->setId('Facebook-OAuth');

$identityProvidersIdentityProvider1->setType('Facebook');

$identityProvidersIdentityProvider1->setName('Facebook');


$identityProvidersArray []= $identityProvidersIdentityProvider1;
$requestBody->setIdentityProviders($identityProvidersArray);




$requestResult = $graphServiceClient->identity()->b2xUserFlows()->post($requestBody);


```