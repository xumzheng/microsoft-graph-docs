---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Notebook()
request_body.setDisplayName('My Private notebook')



result = await client.me.onenote.notebooks.post(request_body, headers=)


```