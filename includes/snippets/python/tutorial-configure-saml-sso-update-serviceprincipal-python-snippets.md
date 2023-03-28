---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ServicePrincipal();
$requestBody->setPreferredSingleSignOnMode('saml');



$requestResult = $graphServiceClient->servicePrincipalsById('servicePrincipal-id')->patch($requestBody);


```