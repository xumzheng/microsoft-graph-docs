---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new GenerateKeyPostRequestBody();
$requestBody->setUse('sig');

$requestBody->setKty('RSA');

$requestBody->setNbf(1508969811);

$requestBody->setExp(1508969811);



$requestResult = $graphServiceClient->trustFramework()->keySetsById('trustFrameworkKeySet-id')->generateKey()->post($requestBody);


```