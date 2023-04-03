---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UploadPkcs12PostRequestBody();
requestBody.setKey('Base64-encoded-pfx-content');

requestBody.setPassword('password-value');



result = await client.trustFramework().keySetsById('trustFrameworkKeySet-id').uploadPkcs12().post(requestBody);


```