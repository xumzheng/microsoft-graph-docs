---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Attachment()
request_body.set@odatatype('#microsoft.graph.referenceAttachment')

request_body.setName('Personal pictures')

additionalData = [
'sourceUrl' => 'https://contoso.com/personal/mario_contoso_net/Documents/Pics', 
'providerType' => 'oneDriveConsumer', 
'permission' => 'Edit', 
'isFolder' => 'True', 
];
request_body.setAdditionalData(additionalData)




result = await client.me.eventsById('event-id').attachments.post(request_body)


```