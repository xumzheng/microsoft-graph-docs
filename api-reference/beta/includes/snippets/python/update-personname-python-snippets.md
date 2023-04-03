---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PersonName();
requestBody.setNickname('Kesha');



result = await client.me().profile().namesById('personName-id').patch(requestBody);


```