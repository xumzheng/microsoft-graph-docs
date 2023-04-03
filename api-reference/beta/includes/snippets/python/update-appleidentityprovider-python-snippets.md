---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = IdentityProviderBase();
requestBody.set@odatatype('#microsoft.graph.socialIdentityProvider');

requestBody.setDisplayName('Apple');



result = awaitclient.identity().identityProvidersById('identityProviderBase-id').patch(requestBody);


```