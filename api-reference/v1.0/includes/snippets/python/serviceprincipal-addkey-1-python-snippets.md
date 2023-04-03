---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AddKeyPostRequestBody();
keyCredential = KeyCredential();
keyCredential.setType('AsymmetricX509Cert');

keyCredential.setUsage('Verify');

KeyCredential.setKey(base64_decode('MIIDYDCCAki...'));


requestBody.setKeyCredential($keyCredential);
requestBody.setPasswordCredential(null);

requestBody.setProof('eyJ0eXAiOiJ...');



requestResult = graphServiceClient.servicePrincipalsById('servicePrincipal-id').addKey().post(requestBody);


```