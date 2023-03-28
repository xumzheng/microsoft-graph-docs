---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new IdentityProvider();
$additionalData = [
'@odata.id' => 'https://graph.microsoft.com/v1.0/identityProviders/Facebook-OAUTH', 
];
$requestBody->setAdditionalData($additionalData);




$graphServiceClient->identity()->b2xUserFlowsById('b2xIdentityUserFlow-id')->identityProvidersById('identityProvider-id')->post($requestBody);


```