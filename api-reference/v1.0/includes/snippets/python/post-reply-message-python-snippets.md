---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ChatMessage();
body = ItemBody();
body.setContentType(BodyType('html'));

body.setContent('Hello World');


requestBody.setBody($body);


result = await client.teamsById('team-id').channelsById('channel-id').messagesById('chatMessage-id').replies().post(requestBody);


```