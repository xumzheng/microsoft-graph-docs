---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrintTaskDefinition()
request_body.displayName = 'Test TaskDefinitionName'

created_by = AppIdentity()
createdBy.displayName = 'Requesting App Display Name'


request_body.created_by = createdBy



result = await client.print.taskDefinitions.post(request_body = request_body)


```