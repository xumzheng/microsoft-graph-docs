---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CreateForwardPostRequestBody()
message = Message()
message.is_delivery_receipt_requested = True

to_recipients_recipient1 = Recipient()
to_recipients_recipient1_email_address = EmailAddress()
toRecipientsRecipient1EmailAddress.address = 'danas@contoso.onmicrosoft.com'

toRecipientsRecipient1EmailAddress.name = 'Dana Swope'


toRecipientsRecipient1.email_address = toRecipientsRecipient1EmailAddress

toRecipientsArray []= toRecipientsRecipient1;
message.torecipients(toRecipientsArray)



request_body.message = message
request_body.comment = 'Dana, just want to make sure you get this; you\'ll need this if the project gets approved.'




result = await client.me.messages_by_id('message-id').createForward.post(request_body = request_body)


```