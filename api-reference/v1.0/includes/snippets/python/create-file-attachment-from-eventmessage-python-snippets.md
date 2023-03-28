---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Attachment();
$requestBody.set@odatatype('microsoft.graph.fileAttachment');

$requestBody.setName('name-value');

$requestBody.setContentType('contentType-value');

$requestBody.setIsInline(false);

$additionalData = [
'contentLocation' => 'contentLocation-value', 
'contentBytes' => 'base64-contentBytes-value', 
];
$requestBody.setAdditionalData($additionalData);




$requestResult = $graphServiceClient.me().messagesById('message-id').attachments().post($requestBody);


```