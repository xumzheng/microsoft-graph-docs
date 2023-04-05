---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReplyAllPostRequestBody()
message = Message()
attachmentsAttachment1 = Attachment()
attachmentsAttachment1.set@odatatype('#microsoft.graph.fileAttachment')

attachmentsAttachment1.setName('guidelines.txt')

additionalData = [
'contentBytes' => 'bWFjIGFuZCBjaGVlc2UgdG9kYXk=', 
];
attachmentsAttachment1.setAdditionalData(additionalData)



attachmentsArray []= attachmentsAttachment1;
message.setAttachments(attachmentsArray)



request_body.setMessage($message)
request_body.setComment('Please take a look at the attached guidelines before you decide on the name.')



await client.me.messages_by_id('message-id').replyAll.post(request_body)


```