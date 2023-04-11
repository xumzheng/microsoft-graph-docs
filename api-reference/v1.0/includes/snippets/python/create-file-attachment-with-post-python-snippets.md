---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReplyPostRequestBody()
post = Post()
postBody = ItemBody()
postBody.ContentType(BodyType('text'))

postBody.content = 'Which quarter does that file cover? See my attachment.'


post.body = postBody
attachmentsAttachment1 = Attachment()
attachmentsAttachment1.@odatatype = '#microsoft.graph.fileAttachment'

attachmentsAttachment1.name = 'Another file as attachment'

additionalData = [
'contentBytes' => 'VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu', 
];
attachmentsAttachment1.additionaldata(additionalData)



attachmentsArray []= attachmentsAttachment1;
post.attachments(attachmentsArray)



request_body.post = post


request_configuration = ReplyRequestBuilderPostRequestConfiguration(
)


await client.groups_by_id('group-id').threads_by_id('conversationThread-id').reply.post(request_body = request_body)


```