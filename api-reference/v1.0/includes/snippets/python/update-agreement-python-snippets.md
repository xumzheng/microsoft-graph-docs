---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Agreement();
$requestBody->setDisplayName('All Contoso volunteers - Terms of use');

$requestBody->setIsViewingBeforeAcceptanceRequired(true);



$requestResult = $graphServiceClient->identityGovernance()->termsOfUse()->agreementsById('agreement-id')->patch($requestBody);


```