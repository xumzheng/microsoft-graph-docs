---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Message()
request_body.subject = 'Party planning'

to_recipients_recipient1 = Recipient()
to_recipients_recipient1_email_address = EmailAddress()
toRecipientsRecipient1EmailAddress.name = 'Samantha Booth'

toRecipientsRecipient1EmailAddress.address = 'samanthab@contoso.onmicrosoft.com'


toRecipientsRecipient1.email_address = toRecipientsRecipient1EmailAddress

toRecipientsArray []= toRecipientsRecipient1;
request_body.torecipients(toRecipientsArray)


mentions_mention1 = Mention()
mentions_mention1_mentioned = EmailAddress()
mentionsMention1Mentioned.name = 'Dana Swope'

mentionsMention1Mentioned.address = 'danas@contoso.onmicrosoft.com'


mentionsMention1.mentioned = mentionsMention1Mentioned

mentionsArray []= mentionsMention1;
request_body.mentions(mentionsArray)





result = await client.me.messages.post(request_body = request_body)


```