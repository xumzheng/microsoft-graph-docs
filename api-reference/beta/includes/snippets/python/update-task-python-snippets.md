---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = PrintTask();
status = PrintTaskStatus();
status.setState(PrintTaskProcessingState('completed'));

status.setDescription('completed');


requestBody.setStatus($status);


requestResult = graphServiceClient.print().taskDefinitionsById('printTaskDefinition-id').tasksById('printTask-id').patch(requestBody);


```