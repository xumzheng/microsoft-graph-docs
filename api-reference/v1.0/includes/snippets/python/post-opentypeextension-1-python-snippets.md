---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Message();
requestBody.setSubject('Annual review');

body = ItemBody();
body.setContentType(BodyType('html'));

body.setContent('You should be proud!');


requestBody.setBody($body);
toRecipientsRecipient1 = Recipient();
toRecipientsRecipient1EmailAddress = EmailAddress();
toRecipientsRecipient1EmailAddress.setAddress('rufus@contoso.com');


toRecipientsRecipient1.setEmailAddress($toRecipientsRecipient1EmailAddress);

toRecipientsArray []= toRecipientsRecipient1;
requestBody.setToRecipients(toRecipientsArray);


extensionsExtension1 = Extension();
extensionsExtension1.set@odatatype('microsoft.graph.openTypeExtension');

additionalData = [
'extensionName' => 'Com.Contoso.Referral', 
'companyName' => 'Wingtip Toys', 
'expirationDate' => '2015-12-30T11:00:00.000Z', 
'dealValue' => 10000,
];
extensionsExtension1.setAdditionalData(additionalData);



extensionsArray []= extensionsExtension1;
requestBody.setExtensions(extensionsArray);




result = await client.me().messages().post(requestBody);


```