---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ConfirmCompromisedPostRequestBody();
requestBody.setServicePrincipalIds(['9089a539-a539-9089-39a5-899039a58990', ]);



await client.identityProtection().riskyServicePrincipals().confirmCompromised().post(requestBody);


```