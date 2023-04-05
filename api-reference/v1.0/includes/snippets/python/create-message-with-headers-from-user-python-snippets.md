---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Message()
request_body.setSubject('9/8/2018: concert')

body = ItemBody()
body.setContentType(BodyType('html'))

body.setContent('The group represents Washington.')


request_body.setBody($body)
toRecipientsRecipient1 = Recipient()
toRecipientsRecipient1EmailAddress = EmailAddress()
toRecipientsRecipient1EmailAddress.setAddress('AlexW@contoso.OnMicrosoft.com')


toRecipientsRecipient1.setEmailAddress($toRecipientsRecipient1EmailAddress)

toRecipientsArray []= toRecipientsRecipient1;
request_body.setToRecipients(toRecipientsArray)


internetMessageHeadersInternetMessageHeader1 = InternetMessageHeader()
internetMessageHeadersInternetMessageHeader1.setName('x-custom-header-group-name')

internetMessageHeadersInternetMessageHeader1.setValue('Washington')


internetMessageHeadersArray []= internetMessageHeadersInternetMessageHeader1;
internetMessageHeadersInternetMessageHeader2 = InternetMessageHeader()
internetMessageHeadersInternetMessageHeader2.setName('x-custom-header-group-id')

internetMessageHeadersInternetMessageHeader2.setValue('WA001')


internetMessageHeadersArray []= internetMessageHeadersInternetMessageHeader2;
request_body.setInternetMessageHeaders(internetMessageHeadersArray)




result = await client.me.messages.post(request_body)


```