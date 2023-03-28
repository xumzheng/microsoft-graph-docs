---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new RemoveHoldPostRequestBody();
$requestBody->setIds(['39333641443238353535383731453339', '46333131344239353834433430454335', ]);



$graphServiceClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->noncustodialDataSources()->securityRemoveHold()->post($requestBody);


```