---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Group();
requestBody.setDescription('Self help community for golf');

requestBody.setDisplayName('Golf Assist');

requestBody.setGroupTypes(['Unified', ]);

requestBody.setMailEnabled(true);

requestBody.setMailNickname('golfassist');

requestBody.setSecurityEnabled(false);



result = await client.groups().post(requestBody);


```