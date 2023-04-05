---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReplyPostRequestBody()
post = Post()
postBody = ItemBody()
postBody.setContentType(BodyType('text'))

postBody.setContent('I attached a reference to a file on OneDrive.')


post.setBody($postBody)
attachmentsAttachment1 = Attachment()
attachmentsAttachment1.set@odatatype('#microsoft.graph.referenceAttachment')

attachmentsAttachment1.setName('Personal pictures')

additionalData = [
'sourceUrl' => 'https://contoso.com/personal/mario_contoso_net/Documents/Pics', 
'providerType' => 'oneDriveConsumer', 
'permission' => 'Edit', 
'isFolder' => 'True', 
];
attachmentsAttachment1.setAdditionalData(additionalData)



attachmentsArray []= attachmentsAttachment1;
post.setAttachments(attachmentsArray)



request_body.setPost($post)


await client.groupsby_id('group-id')_threadsby_id('conversationThread-id')_reply.post(request_body)


```