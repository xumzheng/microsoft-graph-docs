---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Group();
requestBody.setDescription('Contoso Life v2.0');

requestBody.setDisplayName('Contoso Life Renewed');



result = await client.groupsById('group-id').patch(requestBody);


```