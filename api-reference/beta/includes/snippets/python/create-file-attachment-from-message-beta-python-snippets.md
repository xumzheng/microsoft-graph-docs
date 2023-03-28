---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Attachment();
$requestBody->set@odatatype('#microsoft.graph.fileAttachment');

$requestBody->setName('smile');

$additionalData = [
'contentBytes' => 'a0b1c76de9f7=', 
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->me()->messagesById('message-id')->attachments()->post($requestBody);


```