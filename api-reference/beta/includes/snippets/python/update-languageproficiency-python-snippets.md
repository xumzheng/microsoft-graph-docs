---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = LanguageProficiency()
request_body.setAllowedAudiences(AllowedAudiences('organization'))



result = await client.me.profile.languagesById('languageProficiency-id').patch(request_body)


```