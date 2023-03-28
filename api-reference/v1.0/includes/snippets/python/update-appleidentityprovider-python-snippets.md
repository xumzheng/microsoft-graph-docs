---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new IdentityProviderBase();
$requestBody->set@odatatype('#microsoft.graph.socialIdentityProvider');

$requestBody->setDisplayName('Apple');



$requestResult = $graphServiceClient->identity()->identityProvidersById('identityProviderBase-id')->patch($requestBody);


```