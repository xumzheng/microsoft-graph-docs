---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Program();
requestBody.setDisplayName('testprogram3');

requestBody.setDescription('test description');



requestResult = graphServiceClient.programs().post(requestBody);


```