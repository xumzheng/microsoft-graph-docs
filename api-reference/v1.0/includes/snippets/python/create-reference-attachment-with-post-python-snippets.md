---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ReplyPostRequestBody();
post = Post();
postBody = ItemBody();
postBody.setContentType(BodyType('text'));

postBody.setContent('I attached a reference to a file on OneDrive.');


post.setBody($postBody);
attachmentsAttachment1 = Attachment();
attachmentsAttachment1.set@odatatype('#microsoft.graph.referenceAttachment');

attachmentsAttachment1.setName('Personal pictures');

additionalData = [
'sourceUrl' => 'https://contoso.com/personal/mario_contoso_net/Documents/Pics', 
'providerType' => 'oneDriveConsumer', 
'permission' => 'Edit', 
'isFolder' => 'True', 
];
attachmentsAttachment1.setAdditionalData(additionalData);



attachmentsArray []= attachmentsAttachment1;
post.setAttachments(attachmentsArray);



requestBody.setPost($post);


awaitclient.groupsById('group-id').threadsById('conversationThread-id').reply().post(requestBody);


```