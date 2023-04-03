---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Group();
requestBody.setDescription('Library Assist');

requestBody.setDisplayName('Library Assist');

requestBody.setGroupTypes(['Unified', ]);

requestBody.setMailEnabled(true);

requestBody.setMailNickname('library-help');



result = await client.groupsById('group-id').patch(requestBody);


```