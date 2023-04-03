---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ChatMessage();
body = ItemBody();
body.setContent('Hello world');


requestBody.setBody($body);


result = await client.chatsById('chat-id').messages().post(requestBody);


```