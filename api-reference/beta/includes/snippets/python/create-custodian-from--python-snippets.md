---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Custodian();
$requestBody.setEmail('AdeleV@contoso.com');

$requestBody.setApplyHoldToSources(true);



$requestResult = $graphServiceClient.compliance().ediscovery().casesById('case-id').custodians().post($requestBody);


```