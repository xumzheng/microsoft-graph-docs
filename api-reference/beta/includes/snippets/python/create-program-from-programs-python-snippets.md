---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Program();
requestBody.setDisplayName('testprogram3');

requestBody.setDescription('test description');



result = await client.programs().post(requestBody);


```