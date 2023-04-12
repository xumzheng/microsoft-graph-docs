---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomSecurityAttributeDefinition()
request_body.attributeSet = 'Engineering'

request_body.description = 'Active projects for user'

request_body.isCollection = true

request_body.isSearchable = true

request_body.name = 'Project'

request_body.status = 'Available'

request_body.type = 'String'

request_body.usePreDefinedValuesOnly = true




result = await client.directory.customSecurityAttributeDefinitions.post(request_body = request_body)


```