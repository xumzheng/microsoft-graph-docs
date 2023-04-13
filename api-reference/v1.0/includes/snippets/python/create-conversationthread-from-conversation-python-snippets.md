---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConversationThread()
request_body.topic = 'Take your wellness days and rest'

posts_post1 = Post()
posts_post1_body = ItemBody()
postsPost1Body.ContentType(BodyType('html'))

postsPost1Body.content = 'Waiting for the summer holidays.'


postsPost1.body = postsPost1Body

postsArray []= postsPost1;
request_body.posts(postsArray)





result = await client.groups_by_id('group-id').conversations_by_id('conversation-id').threads.post(request_body = request_body)


```