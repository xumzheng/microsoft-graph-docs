---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = CopyToNotebookPostRequestBody();
requestBody.setId('id-value');

requestBody.setGroupId('groupId-value');

requestBody.setRenameAs('renameAs-value');



requestResult = graphServiceClient.me().onenote().sectionsById('onenoteSection-id').copyToNotebook().post(requestBody);


```