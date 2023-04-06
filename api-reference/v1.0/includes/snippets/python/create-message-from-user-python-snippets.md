---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Message()
request_body.setSubject('Did you see last night\'s game?')

request_body.setImportance(Importance('low'))

body = ItemBody()
body.setContentType(BodyType('html'))

body.setContent('They were <b>awesome</b>!')


request_body.setBody($body)
toRecipientsRecipient1 = Recipient()
toRecipientsRecipient1EmailAddress = EmailAddress()
toRecipientsRecipient1EmailAddress.setAddress('AdeleV@contoso.onmicrosoft.com')


toRecipientsRecipient1.setEmailAddress($toRecipientsRecipient1EmailAddress)

toRecipientsArray []= toRecipientsRecipient1;
request_body.setToRecipients(toRecipientsArray)




result = await client.me.messages.post(request_body, headers=)


```