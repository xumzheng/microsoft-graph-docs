---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Group();
request_body.setDescription('Self help community for library');

request_body.setDisplayName('Library Assist');

request_body.setGroupTypes(['Unified', ]);

request_body.setMailEnabled(true);

request_body.setMailNickname('library');

request_body.setSecurityEnabled(false);



result = await client.groups.post(request_body);


```