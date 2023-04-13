---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Group()
request_body.description = 'Library Assist'

request_body.displayName = 'Library Assist'

request_body.GroupTypes(['Unified', ])

request_body.mail_enabled = True

request_body.mailNickname = 'library-help'




result = await client.groups_by_id('group-id').patch(request_body = request_body)


```