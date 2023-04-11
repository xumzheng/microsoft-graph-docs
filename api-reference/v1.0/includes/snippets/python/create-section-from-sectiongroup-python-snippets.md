---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OnenoteSection()
request_body.displayName = 'Section name'



request_configuration = SectionsRequestBuilderPostRequestConfiguration(
)


result = await client.me.onenote.sectionGroups_by_id('sectionGroup-id').sections.post(request_body = request_body)


```