---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CopyNotebookPostRequestBody()
request_body.setGroupId('groupId-value')

request_body.setRenameAs('renameAs-value')


request_config = CopyNotebookRequestBuilderPostRequestConfiguration(
request_config = CopyNotebookRequestBuilderPostRequestConfiguration(query_params=)


result = await client.me.onenote.notebooks_by_id('notebook-id').copyNotebook.post(request_body, headers=)


```