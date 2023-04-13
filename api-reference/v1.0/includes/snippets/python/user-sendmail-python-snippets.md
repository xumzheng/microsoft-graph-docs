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
toRecipientsRecipient1EmailAddress.address = 'frannis@contoso.onmicrosoft.com'


toRecipientsRecipient1.emailAddress = toRecipientsRecipient1EmailAddress

toRecipientsArray []= toRecipientsRecipient1;
message.torecipients(toRecipientsArray)


ccRecipientsRecipient1 = Recipient()
ccRecipientsRecipient1EmailAddress = EmailAddress()
ccRecipientsRecipient1EmailAddress.address = 'danas@contoso.onmicrosoft.com'


ccRecipientsRecipient1.emailAddress = ccRecipientsRecipient1EmailAddress

ccRecipientsArray []= ccRecipientsRecipient1;
message.ccrecipients(ccRecipientsArray)



request_body.message = message
request_body.saveToSentItems = false




await client.me.sendMail.post(request_body = request_body)


```