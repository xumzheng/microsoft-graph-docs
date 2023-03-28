---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new EdiscoveryHoldPolicy();
$requestBody->setDescription('updated description');



$requestResult = $graphServiceClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->legalHoldsById('ediscoveryHoldPolicy-id')->patch($requestBody);


```