---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AuthenticationContextClassReference();
$requestBody->setDisplayName('Contoso medium');

$requestBody->setDescription('Medium protection level defined for Contoso policy');

$requestBody->setIsAvailable(true);



$requestResult = $graphServiceClient->identity()->conditionalAccess()->authenticationContextClassReferencesById('authenticationContextClassReference-id')->patch($requestBody);


```