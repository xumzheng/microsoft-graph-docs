---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CreateForwardPostRequestBody()
message = Message()
message.setIsDeliveryReceiptRequested(true)

toRecipientsRecipient1 = Recipient()
toRecipientsRecipient1EmailAddress = EmailAddress()
toRecipientsRecipient1EmailAddress.setAddress('danas@contoso.onmicrosoft.com')

toRecipientsRecipient1EmailAddress.setName('Dana Swope')


toRecipientsRecipient1.setEmailAddress($toRecipientsRecipient1EmailAddress)

toRecipientsArray []= toRecipientsRecipient1;
message.setToRecipients(toRecipientsArray)



request_body.setMessage($message)
request_body.setComment('Dana, just want to make sure you get this; you\'ll need this if the project gets approved.')



result = await client.me.messagesby_id('message-id').createForward.post(request_body)


```