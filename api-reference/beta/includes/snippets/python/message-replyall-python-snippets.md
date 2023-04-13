---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReplyAllPostRequestBody()
message = Message()
attachments_attachment1 = Attachment()
attachmentsAttachment1.@odatatype = '#microsoft.graph.fileAttachment'

attachmentsAttachment1.name = 'guidelines.txt'

additionalData = [
'contentBytes' => 'bWFjIGFuZCBjaGVlc2UgdG9kYXk=', 
];
attachmentsAttachment1.additionaldata(additionalData)



attachmentsArray []= attachmentsAttachment1;
message.attachments(attachmentsArray)



request_body.message = message
request_body.comment = 'Please take a look at the attached guidelines before you decide on the name.'




await client.me.messages_by_id('message-id').replyAll.post(request_body = request_body)


```