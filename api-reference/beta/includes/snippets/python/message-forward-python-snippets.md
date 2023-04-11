---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ForwardPostRequestBody()
message = Message()
message.isDeliveryReceiptRequested = true

toRecipientsRecipient1 = Recipient()
toRecipientsRecipient1EmailAddress = EmailAddress()
toRecipientsRecipient1EmailAddress.address = 'danas@contoso.onmicrosoft.com'

toRecipientsRecipient1EmailAddress.name = 'Dana Swope'


toRecipientsRecipient1.emailAddress = toRecipientsRecipient1EmailAddress

toRecipientsArray []= toRecipientsRecipient1;
message.torecipients(toRecipientsArray)



request_body.message = message
request_body.comment = 'Dana, just want to make sure you get this.'




await client.me.messages_by_id('message-id').forward.post(request_body = request_body)


```