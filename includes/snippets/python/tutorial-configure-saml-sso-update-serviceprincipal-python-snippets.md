---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ServicePrincipal()
request_body.setPreferredSingleSignOnMode('saml')



result = await client.servicePrincipalsById('servicePrincipal-id').patch(request_body)


```