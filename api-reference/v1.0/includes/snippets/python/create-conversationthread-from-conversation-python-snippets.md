---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ConversationThread();
requestBody.setTopic('Take your wellness days and rest');

postsPost1 = Post();
postsPost1Body = ItemBody();
postsPost1Body.setContentType(BodyType('html'));

postsPost1Body.setContent('Waiting for the summer holidays.');


postsPost1.setBody($postsPost1Body);

postsArray []= postsPost1;
requestBody.setPosts(postsArray);




result = awaitclient.groupsById('group-id').conversationsById('conversation-id').threads().post(requestBody);


```