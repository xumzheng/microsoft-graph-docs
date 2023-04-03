---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ReplyAllPostRequestBody();
requestBody.setComment('comment-value');



graphServiceClient.me().messagesById('message-id').replyAll().post(requestBody);


```