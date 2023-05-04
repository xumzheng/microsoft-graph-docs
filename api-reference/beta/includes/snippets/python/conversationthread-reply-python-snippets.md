---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Reply_post_request_body()
post = Post()
postbody = Item_body()
postbody.contenttype(BodyType.Text('bodytype.text'))

postbody.content = 'content-value'


post.body = postbody

request_body.post = post



await client.groups.by_group_id('group-id').threads.by_thread_id('conversationThread-id').reply.post(request_body = request_body)


```