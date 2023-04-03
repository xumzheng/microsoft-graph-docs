---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AttributeSet();
requestBody.setId('Engineering');

requestBody.setDescription('Attributes for engineering team');

requestBody.setMaxAttributesPerSet(25);



requestResult = graphServiceClient.directory().attributeSets().post(requestBody);


```