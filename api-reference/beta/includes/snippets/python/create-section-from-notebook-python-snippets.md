---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OnenoteSection()
request_body.setDisplayName('Section name')



result = await client.me_onenote_notebooksby_id('notebook-id')_sections.post(request_body)


```