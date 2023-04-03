---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AddKeyPostRequestBody();
keyCredential = KeyCredential();
keyCredential.setType('X509CertAndPassword');

keyCredential.setUsage('Sign');

KeyCredential.setKey(base64_decode('MIIDYDCCAki...'));


requestBody.setKeyCredential($keyCredential);
passwordCredential = PasswordCredential();
passwordCredential.setSecretText('MKTr0w1...');


requestBody.setPasswordCredential($passwordCredential);
requestBody.setProof('eyJ0eXAiOiJ...');



result = awaitclient.applicationsById('application-id').addKey().post(requestBody);


```