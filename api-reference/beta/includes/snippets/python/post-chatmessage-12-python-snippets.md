---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ChatMessage();
body = ItemBody();
body.setContentType(BodyType('html'));

body.setContent('<emoji alt=\"😶‍🌫️\"></emoji>');


requestBody.setBody($body);


requestResult = graphServiceClient.chatsById('chat-id').messages().post(requestBody);


```