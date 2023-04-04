---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = IdentityProviderBase();
request_body.set@odatatype('#microsoft.graph.socialIdentityProvider');

request_body.setDisplayName('Apple');



result = await client.identity.identityProvidersById('identityProviderBase-id').patch(request_body);


```