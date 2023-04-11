---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AttributeSet()
request_body.id = 'Engineering'

request_body.description = 'Attributes for engineering team'

request_body.maxAttributesPerSet = 25



request_configuration = AttributeSetsRequestBuilderPostRequestConfiguration(
)


result = await client.directory.attributeSets.post(request_body = request_body)


```