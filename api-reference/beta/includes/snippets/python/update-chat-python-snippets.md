---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Chat();
requestBody.setTopic('Group chat title update');



result = awaitclient.chatsById('chat-id').patch(requestBody);


```