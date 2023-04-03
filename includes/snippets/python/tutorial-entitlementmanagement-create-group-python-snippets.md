---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Group();
requestBody.setDescription('Marketing group');

requestBody.setDisplayName('Marketing resources');

requestBody.setMailEnabled(false);

requestBody.setMailNickname('markres');

requestBody.setSecurityEnabled(true);



result = await client.groups().post(requestBody);


```