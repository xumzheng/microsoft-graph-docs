---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Group();
requestBody.setDisplayName('myGroup');



requestResult = graphServiceClient.termStore().groups().post(requestBody);


```