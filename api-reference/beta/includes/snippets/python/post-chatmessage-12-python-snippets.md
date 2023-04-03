---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ChatMessage();
body = ItemBody();
body.setContentType(BodyType('html'));

body.setContent('<emoji alt=\"😶‍🌫️\"></emoji>');


requestBody.setBody($body);


result = awaitclient.chatsById('chat-id').messages().post(requestBody);


```