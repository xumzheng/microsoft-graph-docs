---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomSecurityAttributeDefinition()
request_body.setStatus('Deprecated')



result = await client.directory_customSecurityAttributeDefinitionsby_id('customSecurityAttributeDefinition-id').patch(request_body)


```