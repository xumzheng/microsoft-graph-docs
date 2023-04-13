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

postBody.content = 'I attached a reference to a file on OneDrive.'


post.body = postBody
attachmentsAttachment1 = Attachment()
attachmentsAttachment1.@odatatype = '#microsoft.graph.referenceAttachment'

attachmentsAttachment1.name = 'Personal pictures'

additionalData = [
'sourceUrl' => 'https://contoso.com/personal/mario_contoso_net/Documents/Pics', 
'providerType' => 'oneDriveConsumer', 
'permission' => 'Edit', 
'isFolder' => 'True', 
];
attachmentsAttachment1.additionaldata(additionalData)



attachmentsArray []= attachmentsAttachment1;
post.attachments(attachmentsArray)



request_body.post = post



await client.groups_by_id('group-id').threads_by_id('conversationThread-id').reply.post(request_body = request_body)


```