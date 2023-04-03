---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = UploadSecretPostRequestBody();
requestBody.setUse('use-value');

requestBody.setK('application-secret-to-be-uploaded');

requestBody.setNbf(1508969811);

requestBody.setExp(1508973711);



requestResult = graphServiceClient.trustFramework().keySetsById('trustFrameworkKeySet-id').uploadSecret().post(requestBody);


```