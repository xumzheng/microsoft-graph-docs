---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SectionGroup()
request_body.displayName = 'Section group name'




result = await client.me.onenote.notebooks_by_id('notebook-id').sectionGroups.post(request_body = request_body)


```