---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = UploadPkcs12PostRequestBody();
requestBody.setKey('Base64-encoded-pfx-content');

requestBody.setPassword('password-value');



requestResult = graphServiceClient.trustFramework().keySetsById('trustFrameworkKeySet-id').uploadPkcs12().post(requestBody);


```