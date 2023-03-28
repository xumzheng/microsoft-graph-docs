---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CopyPostRequestBody();
$requestBody->setDestinationId('destinationId-value');



$requestResult = $graphServiceClient->me()->mailFoldersById('mailFolder-id')->copy()->post($requestBody);


```