---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = GetPasswordSingleSignOnCredentialsPostRequestBody();
requestBody.setId('5793aa3b-cca9-4794-679a240f8b58');



requestResult = graphServiceClient.servicePrincipalsById('servicePrincipal-id').getPasswordSingleSignOnCredentials().post(requestBody);


```