---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Message()
request_body.subject = '9/8/2018: concert'

body = ItemBody()
body.ContentType(BodyType('html'))

body.content = 'The group represents Washington.'


request_body.body = body
toRecipientsRecipient1 = Recipient()
toRecipientsRecipient1EmailAddress = EmailAddress()
toRecipientsRecipient1EmailAddress.address = 'AlexW@contoso.OnMicrosoft.com'


toRecipientsRecipient1.emailAddress = toRecipientsRecipient1EmailAddress

toRecipientsArray []= toRecipientsRecipient1;
request_body.torecipients(toRecipientsArray)


internetMessageHeadersInternetMessageHeader1 = InternetMessageHeader()
internetMessageHeadersInternetMessageHeader1.name = 'x-custom-header-group-name'

internetMessageHeadersInternetMessageHeader1.value = 'Washington'


internetMessageHeadersArray []= internetMessageHeadersInternetMessageHeader1;
internetMessageHeadersInternetMessageHeader2 = InternetMessageHeader()
internetMessageHeadersInternetMessageHeader2.name = 'x-custom-header-group-id'

internetMessageHeadersInternetMessageHeader2.value = 'WA001'


internetMessageHeadersArray []= internetMessageHeadersInternetMessageHeader2;
request_body.internetmessageheaders(internetMessageHeadersArray)




request_configuration = MessagesRequestBuilderPostRequestConfiguration(
)


result = await client.me.messages.post(request_body = request_body)


```