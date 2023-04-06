---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendMailPostRequestBody()
message = Message()
message.setSubject('Meet for lunch?')

messageBody = ItemBody()
messageBody.setContentType(BodyType('text'))

messageBody.setContent('The new cafeteria is open.')


message.setBody($messageBody)
toRecipientsRecipient1 = Recipient()
toRecipientsRecipient1EmailAddress = EmailAddress()
toRecipientsRecipient1EmailAddress.setAddress('samanthab@contoso.onmicrosoft.com')


toRecipientsRecipient1.setEmailAddress($toRecipientsRecipient1EmailAddress)

toRecipientsArray []= toRecipientsRecipient1;
message.setToRecipients(toRecipientsArray)


ccRecipientsRecipient1 = Recipient()
ccRecipientsRecipient1EmailAddress = EmailAddress()
ccRecipientsRecipient1EmailAddress.setAddress('danas@contoso.onmicrosoft.com')


ccRecipientsRecipient1.setEmailAddress($ccRecipientsRecipient1EmailAddress)

ccRecipientsArray []= ccRecipientsRecipient1;
message.setCcRecipients(ccRecipientsArray)



request_body.setMessage($message)
request_body.setSaveToSentItems(false)



await client.me.sendMail.post(request_body, headers=)


```