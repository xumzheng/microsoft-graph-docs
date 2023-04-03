---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Message();
requestBody.setIsRead(true);



result = await client.me().messagesById('message-id').patch(requestBody);


```