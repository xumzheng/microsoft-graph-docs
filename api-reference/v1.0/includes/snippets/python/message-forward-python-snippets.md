---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ForwardPostRequestBody()
request_body.comment = 'comment-value'

to_recipients_recipient1 = Recipient()
to_recipients_recipient1_email_address = EmailAddress()
toRecipientsRecipient1EmailAddress.name = 'name-value'

toRecipientsRecipient1EmailAddress.address = 'address-value'


toRecipientsRecipient1.email_address = toRecipientsRecipient1EmailAddress

toRecipientsArray []= toRecipientsRecipient1;
request_body.torecipients(toRecipientsArray)





await client.me.messages_by_id('message-id').forward.post(request_body = request_body)


```