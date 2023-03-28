---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PrintTask();
$status = new PrintTaskStatus();
$status->setState(new PrintTaskProcessingState('completed'));

$status->setDescription('completed');


$requestBody->setStatus($status);


$requestResult = $graphServiceClient->print()->taskDefinitionsById('printTaskDefinition-id')->tasksById('printTask-id')->patch($requestBody);


```