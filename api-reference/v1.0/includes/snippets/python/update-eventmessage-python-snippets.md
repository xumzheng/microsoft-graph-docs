---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Message();
requestBody.setIsRead(true);



result = awaitclient.me().messagesById('message-id').patch(requestBody);


```