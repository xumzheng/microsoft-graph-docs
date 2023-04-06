---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Extension()
request_body.set@odatatype('microsoft.graph.openTypeExtension')

additionalData = [
'extensionName' => 'com.contoso.roamingSettings', 
'theme' => 'dark', 
'color' => 'purple', 
'lang' => 'Japanese', 
];
request_body.setAdditionalData(additionalData)



request_config = ExtensionsRequestBuilderPostRequestConfiguration(
request_config = ExtensionsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.me.extensions.post(request_body, headers=)


```