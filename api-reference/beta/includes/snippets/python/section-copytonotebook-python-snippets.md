---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = CopyToNotebookPostRequestBody();
request_body.setId('id-value');

request_body.setGroupId('groupId-value');

request_body.setRenameAs('renameAs-value');



result = await client.me().onenote().sectionsById('onenoteSection-id').copyToNotebook().post(request_body);


```