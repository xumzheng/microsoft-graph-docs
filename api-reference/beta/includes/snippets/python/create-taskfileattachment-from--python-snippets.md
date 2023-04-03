---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AttachmentBase();
requestBody.set@odatatype('#microsoft.graph.taskFileAttachment');

requestBody.setName('smile');

requestBody.setContentType('image/gif');

additionalData = [
'contentBytes' => 'a0b1c76de9f7=', 
];
requestBody.setAdditionalData(additionalData);




result = await client.me().todo().listsById('todoTaskList-id').tasksById('todoTask-id').attachments().post(requestBody);


```