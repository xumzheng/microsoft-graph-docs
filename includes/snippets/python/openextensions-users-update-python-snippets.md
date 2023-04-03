---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Extension();
additionalData = [
'theme' => 'light', 
'color' => 'yellow', 
'lang' => 'Swahili', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.me().extensionsById('extension-id').patch(requestBody);


```