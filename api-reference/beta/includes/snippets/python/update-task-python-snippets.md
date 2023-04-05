---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrintTask()
status = PrintTaskStatus()
status.setState(PrintTaskProcessingState('completed'))

status.setDescription('completed')


request_body.setStatus($status)


result = await client.print.taskDefinitions._by_id('printTaskDefinition-id').tasks._by_id('printTask-id').patch(request_body)


```