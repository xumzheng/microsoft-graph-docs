---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Extension();
additionalData = [
'theme' => 'light', 
'color' => 'yellow', 
'lang' => 'Swahili', 
];
requestBody.setAdditionalData(additionalData);




result = await client.me().extensionsById('extension-id').patch(requestBody);


```