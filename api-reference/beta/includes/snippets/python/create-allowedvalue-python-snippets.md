---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AllowedValue()
request_body.setId('Alpine')

request_body.setIsActive(true)



result = await client.directory.customSecurityAttributeDefinitionsby_id('customSecurityAttributeDefinition-id').allowedValues.post(request_body)


```