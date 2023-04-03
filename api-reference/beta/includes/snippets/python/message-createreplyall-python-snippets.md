---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CreateReplyAllPostRequestBody();
message = Message();
attachmentsAttachment1 = Attachment();
attachmentsAttachment1.set@odatatype('#microsoft.graph.fileAttachment');

attachmentsAttachment1.setName('guidelines.txt');

additionalData = [
'contentBytes' => 'bWFjIGFuZCBjaGVlc2UgdG9kYXk=', 
];
attachmentsAttachment1.setAdditionalData(additionalData);



attachmentsArray []= attachmentsAttachment1;
message.setAttachments(attachmentsArray);



requestBody.setMessage($message);
requestBody.setComment('if the project gets approved, please take a look at the attached guidelines before you decide on the name.');



result = await client.me().messagesById('message-id').createReplyAll().post(requestBody);


```