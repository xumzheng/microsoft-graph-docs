---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DeletePasswordSingleSignOnCredentialsPostRequestBody()
request_body.setId('5793aa3b-cca9-4794-679a240f8b58')



await client.servicePrincipals_by_id('servicePrincipal-id').deletePasswordSingleSignOnCredentials.post(request_body)


```