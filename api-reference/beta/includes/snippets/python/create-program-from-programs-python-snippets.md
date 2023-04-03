---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Program();
requestBody.setDisplayName('testprogram3');

requestBody.setDescription('test description');



result = awaitclient.programs().post(requestBody);


```