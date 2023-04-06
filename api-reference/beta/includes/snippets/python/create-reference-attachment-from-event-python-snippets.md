---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

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



request_config = AttachmentsRequestBuilderPostRequestConfiguration(
request_config = AttachmentsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.me.events_by_id('event-id').attachments.post(request_body, headers=)


```