---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ReplyAllPostRequestBody();
requestBody.setComment('comment-value');



await client.me().messagesById('message-id').replyAll().post(requestBody);


```