---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Extension();
additionalData = [
'theme' => 'light', 
'color' => 'yellow', 
'lang' => 'Swahili', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.me().extensionsById('extension-id').patch(requestBody);


```