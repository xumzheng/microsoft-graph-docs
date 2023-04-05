---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AttributeSet()
request_body.setId('Engineering')

request_body.setDescription('Attributes for engineering team')

request_body.setMaxAttributesPerSet(25)



result = await client.directory_attributeSets.post(request_body)


```