---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AttributeSet();
requestBody.setId('Engineering');

requestBody.setDescription('Attributes for engineering team');

requestBody.setMaxAttributesPerSet(25);



result = await client.directory().attributeSets().post(requestBody);


```