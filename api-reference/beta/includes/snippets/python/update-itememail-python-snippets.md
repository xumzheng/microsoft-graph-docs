---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ItemEmail()
request_body.setDisplayName('Business Email')

request_body.setType(EmailType('work'))



result = await client.usersby_id('user-id')_profile_emailsby_id('itemEmail-id').patch(request_body)


```