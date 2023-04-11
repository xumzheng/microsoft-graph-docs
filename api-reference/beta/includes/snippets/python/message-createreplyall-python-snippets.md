---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CreateReplyAllPostRequestBody()
message = Message()
attachmentsAttachment1 = Attachment()
attachmentsAttachment1.@odatatype = '#microsoft.graph.fileAttachment'

attachmentsAttachment1.name = 'guidelines.txt'

additionalData = [
'contentBytes' => 'bWFjIGFuZCBjaGVlc2UgdG9kYXk=', 
];
attachmentsAttachment1.additionaldata(additionalData)



attachmentsArray []= attachmentsAttachment1;
message.attachments(attachmentsArray)



request_body.message = message
request_body.comment = 'if the project gets approved, please take a look at the attached guidelines before you decide on the name.'



request_configuration = CreateReplyAllRequestBuilderPostRequestConfiguration(
)


result = await client.me.messages_by_id('message-id').createReplyAll.post(request_body = request_body)


```