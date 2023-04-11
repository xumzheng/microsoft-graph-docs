---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Extension()
request_body.@odatatype = 'microsoft.graph.openTypeExtension'

additionalData = [
'extensionName' => 'Com.Contoso.Deal', 
'companyName' => 'Alpine Skis', 
'dealValue' => 1010100,
'expirationDate' => '2015-07-03T13:04:00.000Z', 
];
request_body.additionaldata(additionalData)




request_configuration = ExtensionsRequestBuilderPostRequestConfiguration(
)


result = await client.groups_by_id('group-id').events_by_id('event-id').extensions.post(request_body = request_body)


```