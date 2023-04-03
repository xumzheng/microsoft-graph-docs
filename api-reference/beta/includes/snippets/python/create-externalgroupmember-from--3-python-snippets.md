---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Identity();
requestBody.setId('1431b9c38ee647f6a');

requestBody.setType(IdentityType('externalgroup'));



result = await client.external().connectionsById('externalConnection-id').groupsById('externalGroup-id').members().post(requestBody);


```