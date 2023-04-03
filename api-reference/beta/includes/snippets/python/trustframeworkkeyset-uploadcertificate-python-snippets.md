---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UploadCertificatePostRequestBody();
requestBody.setKey('key-value');



result = awaitclient.trustFramework().keySetsById('trustFrameworkKeySet-id').uploadCertificate().post(requestBody);


```