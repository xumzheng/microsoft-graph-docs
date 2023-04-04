---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = UploadPkcs12PostRequestBody();
request_body.setKey('Base64-encoded-pfx-content');

request_body.setPassword('password-value');



result = await client.trustFramework().keySetsById('trustFrameworkKeySet-id').uploadPkcs12().post(request_body);


```