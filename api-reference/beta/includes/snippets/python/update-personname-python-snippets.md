---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PersonName();
requestBody.setNickname('Kesha');



result = awaitclient.me().profile().namesById('personName-id').patch(requestBody);


```