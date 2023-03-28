---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Attachment();
$requestBody->set@odatatype('#microsoft.graph.referenceAttachment');

$requestBody->setName('Personal pictures');

$additionalData = [
'sourceUrl' => 'https://contoso.com/personal/mario_contoso_net/Documents/Pics', 
'providerType' => 'oneDriveConsumer', 
'permission' => 'Edit', 
'isFolder' => 'True', 
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->me()->eventsById('event-id')->attachments()->post($requestBody);


```