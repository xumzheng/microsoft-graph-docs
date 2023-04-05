---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConversationThread()
request_body.setTopic('Take your wellness days and rest')

postsPost1 = Post()
postsPost1Body = ItemBody()
postsPost1Body.setContentType(BodyType('html'))

postsPost1Body.setContent('Waiting for the summer holidays.')


postsPost1.setBody($postsPost1Body)

postsArray []= postsPost1;
request_body.setPosts(postsArray)




result = await client.groupsby_id('group-id')_conversationsby_id('conversation-id')_threads.post(request_body)


```