---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AttachmentBase();
$requestBody->set@odatatype('#microsoft.graph.taskFileAttachment');

$requestBody->setName('smile');

$requestBody->setContentType('image/gif');

$additionalData = [
'contentBytes' => 'a0b1c76de9f7=', 
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->me()->todo()->listsById('todoTaskList-id')->tasksById('todoTask-id')->attachments()->post($requestBody);


```