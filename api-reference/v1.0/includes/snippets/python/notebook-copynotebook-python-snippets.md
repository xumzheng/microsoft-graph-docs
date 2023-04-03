---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CopyNotebookPostRequestBody();
requestBody.setGroupId('groupId-value');

requestBody.setRenameAs('renameAs-value');



result = await client.me().onenote().notebooksById('notebook-id').copyNotebook().post(requestBody);


```