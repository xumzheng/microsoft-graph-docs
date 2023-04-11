---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Message()
request_body.subject = 'Party planning'

toRecipientsRecipient1 = Recipient()
toRecipientsRecipient1EmailAddress = EmailAddress()
toRecipientsRecipient1EmailAddress.name = 'Samantha Booth'

toRecipientsRecipient1EmailAddress.address = 'samanthab@contoso.onmicrosoft.com'


toRecipientsRecipient1.emailAddress = toRecipientsRecipient1EmailAddress

toRecipientsArray []= toRecipientsRecipient1;
request_body.torecipients(toRecipientsArray)


mentionsMention1 = Mention()
mentionsMention1Mentioned = EmailAddress()
mentionsMention1Mentioned.name = 'Dana Swope'

mentionsMention1Mentioned.address = 'danas@contoso.onmicrosoft.com'


mentionsMention1.mentioned = mentionsMention1Mentioned

mentionsArray []= mentionsMention1;
request_body.mentions(mentionsArray)




request_configuration = MessagesRequestBuilderPostRequestConfiguration(
)


result = await client.me.messages.post(request_body = request_body)


```