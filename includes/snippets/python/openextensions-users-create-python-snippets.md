---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Extension();
requestBody.set@odatatype('microsoft.graph.openTypeExtension');

additionalData = [
'extensionName' => 'com.contoso.roamingSettings', 
'theme' => 'dark', 
'color' => 'purple', 
'lang' => 'Japanese', 
];
requestBody.setAdditionalData(additionalData);




result = await client.me().extensions().post(requestBody);


```