---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Message()
request_body.subject = 'Annual review'

body = ItemBody()
body.ContentType(BodyType('html'))

body.content = 'You should be proud!'


request_body.body = body
to_recipients_recipient1 = Recipient()
to_recipients_recipient1_email_address = EmailAddress()
toRecipientsRecipient1EmailAddress.address = 'rufus@contoso.com'


toRecipientsRecipient1.email_address = toRecipientsRecipient1EmailAddress

toRecipientsArray []= toRecipientsRecipient1;
request_body.torecipients(toRecipientsArray)


extensions_extension1 = Extension()
extensionsExtension1.@odatatype = 'microsoft.graph.openTypeExtension'

additionalData = [
'extensionName' => 'Com.Contoso.Referral', 
'companyName' => 'Wingtip Toys', 
'expirationDate' => '2015-12-30T11:00:00.000Z', 
'dealValue' => 10000,
];
extensionsExtension1.additionaldata(additionalData)



extensionsArray []= extensionsExtension1;
request_body.extensions(extensionsArray)





result = await client.me.messages.post(request_body = request_body)


```