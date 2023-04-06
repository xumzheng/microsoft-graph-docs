---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Extension()
additionalData = [
'theme' => 'light', 
'color' => 'yellow', 
'lang' => 'Swahili', 
];
request_body.setAdditionalData(additionalData)



request_config = ExtensionRequestBuilderPatchRequestConfiguration(
request_config = ExtensionRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.me.extensions_by_id('extension-id').patch(request_body, headers=)


```