---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = MovePostRequestBody();
requestBody.setDestinationId('deleteditems');



result = await client.me().messagesById('message-id').move().post(requestBody);


```