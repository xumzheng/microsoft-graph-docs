---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ReplyPostRequestBody();
post = Post();
postBody = ItemBody();
postBody.setContentType(BodyType('text'));

postBody.setContent('Which quarter does that file cover? See my attachment.');


post.setBody($postBody);
attachmentsAttachment1 = Attachment();
attachmentsAttachment1.set@odatatype('#microsoft.graph.fileAttachment');

attachmentsAttachment1.setName('Another file as attachment');

additionalData = [
'contentBytes' => 'VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu', 
];
attachmentsAttachment1.setAdditionalData(additionalData);



attachmentsArray []= attachmentsAttachment1;
post.setAttachments(attachmentsArray);



request_body.setPost($post);


await client.groupsById('group-id').threadsById('conversationThread-id').reply().post(request_body);


```