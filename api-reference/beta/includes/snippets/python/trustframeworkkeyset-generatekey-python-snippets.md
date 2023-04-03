---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = GenerateKeyPostRequestBody();
requestBody.setUse('sig');

requestBody.setKty('RSA');

requestBody.setNbf(1508969811);

requestBody.setExp(1508969811);



result = awaitclient.trustFramework().keySetsById('trustFrameworkKeySet-id').generateKey().post(requestBody);


```