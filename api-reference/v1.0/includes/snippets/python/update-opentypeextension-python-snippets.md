---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Extension()
request_body.@odatatype = 'Microsoft.OutlookServices.OpenTypeExtension'

additionalData = [
'extensionName' => 'Com.Contoso.Estimate', 
'companyName' => 'Contoso', 
'expirationDate' => '2016-07-30T11:00:00.000Z', 
'DealValue' => 1010100,
'topPicks' => ['Employees only', 'Add spouse or guest', 'Add family', ],
];
request_body.additionaldata(additionalData)





result = await client.groups_by_id('group-id').threads_by_id('conversationThread-id').posts_by_id('post-id').extensions_by_id('extension-id').patch(request_body = request_body)


```