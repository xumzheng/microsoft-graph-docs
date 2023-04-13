---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AttributeSet()
request_body.description = 'Attributes for engineering team'

request_body.max_attributes_per_set = 20




result = await client.directory.attributeSets_by_id('attributeSet-id').patch(request_body = request_body)


```