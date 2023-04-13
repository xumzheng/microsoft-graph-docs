---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReplyPostRequestBody()
message = Message()
toRecipientsRecipient1 = Recipient()
toRecipientsRecipient1EmailAddress = EmailAddress()
toRecipientsRecipient1EmailAddress.address = 'samanthab@contoso.onmicrosoft.com'

toRecipientsRecipient1EmailAddress.name = 'Samantha Booth'


toRecipientsRecipient1.emailAddress = toRecipientsRecipient1EmailAddress

toRecipientsArray []= toRecipientsRecipient1;
toRecipientsRecipient2 = Recipient()
toRecipientsRecipient2EmailAddress = EmailAddress()
toRecipientsRecipient2EmailAddress.address = 'randiw@contoso.onmicrosoft.com'

toRecipientsRecipient2EmailAddress.name = 'Randi Welch'


toRecipientsRecipient2.emailAddress = toRecipientsRecipient2EmailAddress

toRecipientsArray []= toRecipientsRecipient2;
message.torecipients(toRecipientsArray)



request_body.message = message
request_body.comment = 'Samantha, Randi, would you name the group please?'




await client.me.messages_by_id('message-id').reply.post(request_body = request_body)


```