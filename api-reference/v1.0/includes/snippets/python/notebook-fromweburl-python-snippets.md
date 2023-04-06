---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetNotebookFromWebUrlPostRequestBody()
request_body.setWebUrl('webUrl value')



result = await client.me.onenote.notebooks.getNotebookFromWebUrl.post(request_body, headers=)


```