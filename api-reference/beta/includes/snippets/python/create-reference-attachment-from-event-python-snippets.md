---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Attachment();
requestBody.set@odatatype('#microsoft.graph.referenceAttachment');

requestBody.setName('Personal pictures');

additionalData = [
'sourceUrl' => 'https://contoso.com/personal/mario_contoso_net/Documents/Pics', 
'providerType' => 'oneDriveConsumer', 
'permission' => 'Edit', 
'isFolder' => 'True', 
];
requestBody.setAdditionalData(additionalData);




result = await client.me().eventsById('event-id').attachments().post(requestBody);


```