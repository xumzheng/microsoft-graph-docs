---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AddTokenSigningCertificatePostRequestBody();
requestBody.setDisplayName('CN=customDisplayName');

requestBody.setEndDateTime(DateTime('2024-01-25T00:00:00Z'));



requestResult = graphServiceClient.servicePrincipalsById('servicePrincipal-id').addTokenSigningCertificate().post(requestBody);


```