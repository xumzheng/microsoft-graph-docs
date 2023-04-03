---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ServicePrincipal();
requestBody.setPreferredSingleSignOnMode('saml');



result = awaitclient.servicePrincipalsById('servicePrincipal-id').patch(requestBody);


```