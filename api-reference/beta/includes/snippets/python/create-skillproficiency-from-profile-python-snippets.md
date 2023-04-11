---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SkillProficiency()
request_body.Categories(['Professional', ])

request_body.AllowedAudiences(AllowedAudiences('organization'))

request_body.displayName = 'API Design'

request_body.Proficiency(SkillProficiencyLevel('generalprofessional'))

request_body.CollaborationTags(['ableToMentor', ])




result = await client.me.profile.skills.post(request_body = request_body)


```