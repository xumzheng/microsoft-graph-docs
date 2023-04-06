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



request_config = ThreadsRequestBuilderPostRequestConfiguration(
request_config = ThreadsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.groups_by_id('group-id').conversations_by_id('conversation-id').threads.post(request_body, headers=)


```