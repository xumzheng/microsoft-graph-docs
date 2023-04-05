---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SkillProficiency()
request_body.setCategories(['Professional', ])

request_body.setProficiency(SkillProficiencyLevel('advancedprofessional'))



result = await client.me_profile_skillsby_id('skillProficiency-id').patch(request_body)


```