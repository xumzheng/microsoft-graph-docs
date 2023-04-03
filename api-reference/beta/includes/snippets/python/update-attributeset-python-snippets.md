---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AttributeSet();
requestBody.setDescription('Attributes for engineering team');

requestBody.setMaxAttributesPerSet(20);



result = awaitclient.directory().attributeSetsById('attributeSet-id').patch(requestBody);


```