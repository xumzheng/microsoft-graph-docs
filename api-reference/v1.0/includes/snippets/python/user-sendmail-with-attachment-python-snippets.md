---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = SendMailPostRequestBody()
message = Message()
message.setSubject('Meet for lunch?')

messageBody = ItemBody()
messageBody.setContentType(BodyType('text'))

messageBody.setContent('The new cafeteria is open.')


message.setBody($messageBody)
toRecipientsRecipient1 = Recipient()
toRecipientsRecipient1EmailAddress = EmailAddress()
toRecipientsRecipient1EmailAddress.setAddress('meganb@contoso.onmicrosoft.com')


toRecipientsRecipient1.setEmailAddress($toRecipientsRecipient1EmailAddress)

toRecipientsArray []= toRecipientsRecipient1;
message.setToRecipients(toRecipientsArray)


attachmentsAttachment1 = Attachment()
attachmentsAttachment1.set@odatatype('#microsoft.graph.fileAttachment')

attachmentsAttachment1.setName('attachment.txt')

attachmentsAttachment1.setContentType('text/plain')

additionalData = [
'contentBytes' => 'SGVsbG8gV29ybGQh', 
];
attachmentsAttachment1.setAdditionalData(additionalData)



attachmentsArray []= attachmentsAttachment1;
message.setAttachments(attachmentsArray)



request_body.setMessage($message)


await client.me.sendMail.post(request_body)


```