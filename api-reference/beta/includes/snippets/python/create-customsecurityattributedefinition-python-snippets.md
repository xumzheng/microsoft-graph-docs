---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomSecurityAttributeDefinition()
request_body.setAttributeSet('Engineering')

request_body.setDescription('Target completion date')

request_body.setIsCollection(false)

request_body.setIsSearchable(true)

request_body.setName('ProjectDate')

request_body.setStatus('Available')

request_body.setType('String')

request_body.setUsePreDefinedValuesOnly(false)



result = await client.directory_customSecurityAttributeDefinitions.post(request_body)


```