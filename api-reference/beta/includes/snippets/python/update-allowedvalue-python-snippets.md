---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AllowedValue()
request_body.setIsActive(false)



result = await client.directory.customSecurityAttributeDefinitions_by_id('customSecurityAttributeDefinition-id').allowedValues_by_id('allowedValue-id').patch(request_body, headers=)


```