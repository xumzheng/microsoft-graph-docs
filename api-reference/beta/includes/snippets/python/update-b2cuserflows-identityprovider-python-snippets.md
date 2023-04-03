---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ReferenceCreate();
requestBody.set@odataid('https://graph.microsoft.com/beta/identityProviders/{id}');



awaitclient.identity().b2cUserFlowsById('b2cIdentityUserFlow-id').identityProviders().ref().post(requestBody);


```