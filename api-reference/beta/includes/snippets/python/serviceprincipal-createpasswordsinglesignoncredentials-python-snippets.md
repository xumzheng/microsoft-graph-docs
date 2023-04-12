---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CreatePasswordSingleSignOnCredentialsPostRequestBody()
request_body.id = '5793aa3b-cca9-4794-679a240f8b58'

credentialsCredential1 = Credential()
credentialsCredential1.fieldId = 'param_username'

credentialsCredential1.value = 'myusername'

credentialsCredential1.type = 'username'


credentialsArray []= credentialsCredential1;
credentialsCredential2 = Credential()
credentialsCredential2.fieldId = 'param_password'

credentialsCredential2.value = 'pa$$w0rd'

credentialsCredential2.type = 'password'


credentialsArray []= credentialsCredential2;
request_body.credentials(credentialsArray)





result = await client.servicePrincipals_by_id('servicePrincipal-id').createPasswordSingleSignOnCredentials.post(request_body = request_body)


```