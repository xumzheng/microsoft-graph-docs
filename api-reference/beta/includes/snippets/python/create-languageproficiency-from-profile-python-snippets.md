---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = LanguageProficiency()
request_body.displayName = 'Norwegian Bokmål'

request_body.tag = 'nb-NO'

request_body.Spoken(LanguageProficiencyLevel('nativeorbilingual'))

request_body.Written(LanguageProficiencyLevel('nativeorbilingual'))

request_body.Reading(LanguageProficiencyLevel('nativeorbilingual'))




result = await client.me.profile.languages.post(request_body = request_body)


```