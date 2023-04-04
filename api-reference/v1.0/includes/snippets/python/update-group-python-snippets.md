---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Group();
request_body.setDescription('Library Assist');

request_body.setDisplayName('Library Assist');

request_body.setGroupTypes(['Unified', ]);

request_body.setMailEnabled(true);

request_body.setMailNickname('library-help');



result = await client.groupsById('group-id').patch(request_body);


```