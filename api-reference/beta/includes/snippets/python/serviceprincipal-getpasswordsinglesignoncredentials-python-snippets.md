---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = GetPasswordSingleSignOnCredentialsPostRequestBody();
requestBody.setId('5793aa3b-cca9-4794-679a240f8b58');



result = awaitclient.servicePrincipalsById('servicePrincipal-id').getPasswordSingleSignOnCredentials().post(requestBody);


```