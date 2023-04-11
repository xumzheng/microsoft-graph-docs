---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Message()
request_body.subject = 'Did you see last night\'s game?'

request_body.Importance(Importance('low'))

body = ItemBody()
body.ContentType(BodyType('html'))

body.content = 'They were <b>awesome</b>!'


request_body.body = body
toRecipientsRecipient1 = Recipient()
toRecipientsRecipient1EmailAddress = EmailAddress()
toRecipientsRecipient1EmailAddress.address = 'AdeleV@contoso.onmicrosoft.com'


toRecipientsRecipient1.emailAddress = toRecipientsRecipient1EmailAddress

toRecipientsArray []= toRecipientsRecipient1;
request_body.torecipients(toRecipientsArray)




request_configuration = MessagesRequestBuilderPostRequestConfiguration(
)


result = await client.me.messages.post(request_body = request_body)


```