---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CopyNotebookPostRequestBody()
request_body.setGroupId('groupId-value')

request_body.setRenameAs('renameAs-value')



result = await client.me_onenote_notebooksby_id('notebook-id')_copyNotebook.post(request_body)


```