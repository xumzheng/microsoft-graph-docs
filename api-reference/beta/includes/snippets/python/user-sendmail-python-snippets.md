---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendMailPostRequestBody()
message = Message()
message.subject = 'Meet for lunch?'

message_body = ItemBody()
messageBody.ContentType(BodyType('text'))

messageBody.content = 'The new cafeteria is open.'


message.body = messageBody
to_recipients_recipient1 = Recipient()
to_recipients_recipient1_email_address = EmailAddress()
toRecipientsRecipient1EmailAddress.address = 'samanthab@contoso.onmicrosoft.com'


toRecipientsRecipient1.email_address = toRecipientsRecipient1EmailAddress

toRecipientsArray []= toRecipientsRecipient1;
message.torecipients(toRecipientsArray)


cc_recipients_recipient1 = Recipient()
cc_recipients_recipient1_email_address = EmailAddress()
ccRecipientsRecipient1EmailAddress.address = 'danas@contoso.onmicrosoft.com'


ccRecipientsRecipient1.email_address = ccRecipientsRecipient1EmailAddress

ccRecipientsArray []= ccRecipientsRecipient1;
message.ccrecipients(ccRecipientsArray)



request_body.message = message
request_body.save_to_sent_items = False




await client.me.sendMail.post(request_body = request_body)


```