---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendMailPostRequestBody()
message = Message()
message.subject = 'Project kickoff'

toRecipientsRecipient1 = Recipient()
toRecipientsRecipient1EmailAddress = EmailAddress()
toRecipientsRecipient1EmailAddress.name = 'Samantha Booth'

toRecipientsRecipient1EmailAddress.address = 'samanthab@contoso.onmicrosoft.com'


toRecipientsRecipient1.emailAddress = toRecipientsRecipient1EmailAddress

toRecipientsArray []= toRecipientsRecipient1;
message.torecipients(toRecipientsArray)


mentionsMention1 = Mention()
mentionsMention1Mentioned = EmailAddress()
mentionsMention1Mentioned.name = 'Dana Swope'

mentionsMention1Mentioned.address = 'danas@contoso.onmicrosoft.com'


mentionsMention1.mentioned = mentionsMention1Mentioned

mentionsArray []= mentionsMention1;
message.mentions(mentionsArray)



request_body.message = message



await client.me.sendMail.post(request_body = request_body)


```