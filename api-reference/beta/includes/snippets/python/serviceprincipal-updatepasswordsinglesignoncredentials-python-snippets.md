---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = UpdatePasswordSingleSignOnCredentialsPostRequestBody();
requestBody.setId('5793aa3b-cca9-4794-679a240f8b58');

credentialsCredential1 = Credential();
credentialsCredential1.setFieldId('param_username');

credentialsCredential1.setValue('myusername');

credentialsCredential1.setType('username');


credentialsArray []= credentialsCredential1;
credentialsCredential2 = Credential();
credentialsCredential2.setFieldId('param_password');

credentialsCredential2.setValue('pa$$w0rd');

credentialsCredential2.setType('password');


credentialsArray []= credentialsCredential2;
requestBody.setCredentials(credentialsArray);




graphServiceClient.servicePrincipalsById('servicePrincipal-id').updatePasswordSingleSignOnCredentials().post(requestBody);


```