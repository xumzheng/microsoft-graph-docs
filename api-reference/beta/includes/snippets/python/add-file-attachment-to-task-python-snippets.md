---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Attachment();
$requestBody.set@odatatype('#microsoft.graph.fileAttachment');

$requestBody.setName('menu.txt');

$additionalData = [
'contentBytes' => 'bWFjIGFuZCBjaGVlc2UgdG9kYXk=', 
];
$requestBody.setAdditionalData($additionalData);




$requestResult = $graphServiceClient.me().outlook().tasksById('outlookTask-id').attachments().post($requestBody);


```