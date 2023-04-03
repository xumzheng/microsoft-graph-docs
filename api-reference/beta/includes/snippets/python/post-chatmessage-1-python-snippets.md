---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ChatMessage();
body = ItemBody();
body.setContent('Hello World');


requestBody.setBody($body);


result = awaitclient.teamsById('team-id').channelsById('channel-id').messages().post(requestBody);


```