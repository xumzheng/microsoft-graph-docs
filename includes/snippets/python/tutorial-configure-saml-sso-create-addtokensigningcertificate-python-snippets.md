---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AddTokenSigningCertificatePostRequestBody();
requestBody.setDisplayName('CN=AWSContoso');

requestBody.setEndDateTime(DateTime('2024-01-25T00:00:00Z'));



result = awaitclient.servicePrincipalsById('servicePrincipal-id').addTokenSigningCertificate().post(requestBody);


```