---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Custodian();
$requestBody->setApplyHoldToSources(false);



$requestResult = $graphServiceClient->compliance()->ediscovery()->casesById('case-id')->custodiansById('custodian-id')->patch($requestBody);


```