---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Identity();
requestBody.setId('e811976d-83df-4cbd-8b9b-5215b18aa874');

requestBody.setType(IdentityType('user'));



result = await client.external().connectionsById('externalConnection-id').groupsById('externalGroup-id').members().post(requestBody);


```