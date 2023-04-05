---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PersonAnnotation()
request_body.setAllowedAudiences(AllowedAudiences('organization'))



result = await client.usersby_id('user-id').profile.notesby_id('personAnnotation-id').patch(request_body)


```