---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Group()
request_body.description = 'Self help community for golf'

request_body.displayName = 'Golf Assist'

request_body.GroupTypes(['Unified', ])

request_body.mailEnabled = true

request_body.mailNickname = 'golfassist'

request_body.securityEnabled = false




result = await client.groups.post(request_body = request_body)


```