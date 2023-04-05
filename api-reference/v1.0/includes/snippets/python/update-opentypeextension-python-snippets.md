---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Extension()
request_body.set@odatatype('Microsoft.OutlookServices.OpenTypeExtension')

additionalData = [
'extensionName' => 'Com.Contoso.Estimate', 
'companyName' => 'Contoso', 
'expirationDate' => '2016-07-30T11:00:00.000Z', 
'DealValue' => 1010100,
'topPicks' => ['Employees only', 'Add spouse or guest', 'Add family', ],
];
request_body.setAdditionalData(additionalData)




result = await client.groupsby_id('group-id').threadsby_id('conversationThread-id').postsby_id('post-id').extensionsby_id('extension-id').patch(request_body)


```