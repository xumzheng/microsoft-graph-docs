---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReplyPostRequestBody()
post = Post()
post_body = ItemBody()
postBody.ContentType(BodyType('text'))

postBody.content = 'content-value'


post.body = postBody

request_body.post = post



await client.groups_by_id('group-id').threads_by_id('conversationThread-id').reply.post(request_body = request_body)


```