---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Extension()
request_body.set@odatatype('microsoft.graph.openTypeExtension')

additionalData = [
'extensionName' => 'Com.Contoso.Referral', 
'companyName' => 'Wingtip Toys', 
'dealValue' => 500050,
'expirationDate' => '2015-12-03T10:00:00.000Z', 
];
request_body.setAdditionalData(additionalData)




result = await client.me.messagesById('message-id').extensions.post(request_body)


```