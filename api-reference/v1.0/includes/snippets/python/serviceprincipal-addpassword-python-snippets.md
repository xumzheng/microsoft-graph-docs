---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AddPasswordPostRequestBody();
passwordCredential = PasswordCredential();
passwordCredential.setDisplayName('Password friendly name');


requestBody.setPasswordCredential($passwordCredential);


result = awaitclient.servicePrincipalsById('servicePrincipal-id').addPassword().post(requestBody);


```