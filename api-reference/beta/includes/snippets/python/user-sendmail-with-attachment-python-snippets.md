---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendMailPostRequestBody()
message = Message()
message.subject = 'Meet for lunch?'

messageBody = ItemBody()
messageBody.ContentType(BodyType('text'))

messageBody.content = 'The new cafeteria is open.'


message.body = messageBody
toRecipientsRecipient1 = Recipient()
toRecipientsRecipient1EmailAddress = EmailAddress()
toRecipientsRecipient1EmailAddress.address = 'meganb@contoso.onmicrosoft.com'


toRecipientsRecipient1.emailAddress = toRecipientsRecipient1EmailAddress

toRecipientsArray []= toRecipientsRecipient1;
message.torecipients(toRecipientsArray)


attachmentsAttachment1 = Attachment()
attachmentsAttachment1.@odatatype = '#microsoft.graph.fileAttachment'

attachmentsAttachment1.name = 'attachment.txt'

attachmentsAttachment1.contentType = 'text/plain'

additionalData = [
'contentBytes' => 'SGVsbG8gV29ybGQh', 
];
attachmentsAttachment1.additionaldata(additionalData)



attachmentsArray []= attachmentsAttachment1;
message.attachments(attachmentsArray)



request_body.message = message


request_configuration = SendMailRequestBuilderPostRequestConfiguration(
)


await client.me.sendMail.post(request_body = request_body)


```