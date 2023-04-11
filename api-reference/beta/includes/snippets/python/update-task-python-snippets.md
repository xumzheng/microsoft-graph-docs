---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrintTask()
status = PrintTaskStatus()
status.State(PrintTaskProcessingState('completed'))

status.description = 'completed'


request_body.status = status


request_configuration = PrintTaskRequestBuilderPatchRequestConfiguration(
)


result = await client.print.taskDefinitions_by_id('printTaskDefinition-id').tasks_by_id('printTask-id').patch(request_body = request_body)


```