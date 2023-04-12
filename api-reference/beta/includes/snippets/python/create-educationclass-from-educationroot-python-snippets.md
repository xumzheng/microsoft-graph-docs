---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationClass()
request_body.description = 'Health Level 1'

request_body.classCode = 'Health 501'

request_body.displayName = 'Health 1'

request_body.externalId = '11019'

request_body.externalName = 'Health Level 1'

request_body.ExternalSource(EducationExternalSource('sis'))

request_body.mailNickname = 'fineartschool.net'




result = await client.education.classes.post(request_body = request_body)


```