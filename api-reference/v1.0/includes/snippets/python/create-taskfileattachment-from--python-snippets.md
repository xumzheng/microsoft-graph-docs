---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AttachmentBase()
request_body.set@odatatype('#microsoft.graph.taskFileAttachment')

request_body.setName('smile')

request_body.setContentType('image/gif')

additionalData = [
'contentBytes' => 'a0b1c76de9f7=', 
];
request_body.setAdditionalData(additionalData)




result = await client.me.todo.lists_by_id('todoTaskList-id').tasks_by_id('todoTask-id').attachments.post(request_body)


```