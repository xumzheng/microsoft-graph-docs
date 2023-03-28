---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new IdentityProvider();
$requestBody.set@odatatype('microsoft.graph.identityProvider');

$requestBody.setName('Login with Amazon');

$requestBody.setType('Amazon');

$requestBody.setClientId('56433757-cadd-4135-8431-2c9e3fd68ae8');

$requestBody.setClientSecret('000000000000');



$requestResult = $graphServiceClient.identityProviders().post($requestBody);


```