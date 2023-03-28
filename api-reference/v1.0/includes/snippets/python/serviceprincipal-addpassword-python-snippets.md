---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AddPasswordPostRequestBody();
$passwordCredential = new PasswordCredential();
$passwordCredential->setDisplayName('Password friendly name');


$requestBody->setPasswordCredential($passwordCredential);


$requestResult = $graphServiceClient->servicePrincipalsById('servicePrincipal-id')->addPassword()->post($requestBody);


```