---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrintTaskDefinition()
request_body.setDisplayName('Test TaskDefinitionName')

createdBy = AppIdentity()
createdBy.setDisplayName('Requesting App Display Name')


request_body.setCreatedBy($createdBy)


result = await client.print.taskDefinitions.post(request_body, headers=)


```