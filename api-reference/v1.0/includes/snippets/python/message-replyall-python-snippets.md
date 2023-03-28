---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ReplyAllPostRequestBody();
$requestBody->setComment('comment-value');



$graphServiceClient->me()->messagesById('message-id')->replyAll()->post($requestBody);


```