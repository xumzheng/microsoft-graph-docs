---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = MovePostRequestBody();
requestBody.setDestinationId('deleteditems');



result = awaitclient.me().messagesById('message-id').move().post(requestBody);


```