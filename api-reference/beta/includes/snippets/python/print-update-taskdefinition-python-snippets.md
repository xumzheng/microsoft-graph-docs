---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrintTaskDefinition()
request_body.displayName = 'Test TaskDefinitionName'

createdBy = AppIdentity()
createdBy.displayName = 'Requesting App Display Name'


request_body.createdBy = createdBy


request_configuration = PrintTaskDefinitionRequestBuilderPatchRequestConfiguration(
)


result = await client.print.taskDefinitions_by_id('printTaskDefinition-id').patch(request_body = request_body)


```