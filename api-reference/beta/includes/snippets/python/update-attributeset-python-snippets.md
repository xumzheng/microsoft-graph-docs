---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AttributeSet();
requestBody.setDescription('Attributes for engineering team');

requestBody.setMaxAttributesPerSet(20);



result = await client.directory().attributeSetsById('attributeSet-id').patch(requestBody);


```