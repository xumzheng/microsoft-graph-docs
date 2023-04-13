---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendMailPostRequestBody()
message = Message()
message.subject = '9/9/2018: concert'

messageBody = ItemBody()
messageBody.ContentType(BodyType('html'))

messageBody.content = 'The group represents Nevada.'


message.body = messageBody
toRecipientsRecipient1 = Recipient()
toRecipientsRecipient1EmailAddress = EmailAddress()
toRecipientsRecipient1EmailAddress.address = 'AlexW@contoso.OnMicrosoft.com'


toRecipientsRecipient1.emailAddress = toRecipientsRecipient1EmailAddress

toRecipientsArray []= toRecipientsRecipient1;
message.torecipients(toRecipientsArray)


internetMessageHeadersInternetMessageHeader1 = InternetMessageHeader()
internetMessageHeadersInternetMessageHeader1.name = 'x-custom-header-group-name'

internetMessageHeadersInternetMessageHeader1.value = 'Nevada'


internetMessageHeadersArray []= internetMessageHeadersInternetMessageHeader1;
internetMessageHeadersInternetMessageHeader2 = InternetMessageHeader()
internetMessageHeadersInternetMessageHeader2.name = 'x-custom-header-group-id'

internetMessageHeadersInternetMessageHeader2.value = 'NV001'


internetMessageHeadersArray []= internetMessageHeadersInternetMessageHeader2;
message.internetmessageheaders(internetMessageHeadersArray)



request_body.message = message



await client.me.sendMail.post(request_body = request_body)


```