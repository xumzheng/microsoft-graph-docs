---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Extension();
requestBody.set@odatatype('microsoft.graph.openTypeExtension');

additionalData = [
'extensionName' => 'Com.Contoso.Referral', 
'companyName' => 'Wingtip Toys', 
'dealValue' => 500050,
'expirationDate' => '2015-12-03T10:00:00.000Z', 
];
requestBody.setAdditionalData(additionalData);




result = await client.me().messagesById('message-id').extensions().post(requestBody);


```