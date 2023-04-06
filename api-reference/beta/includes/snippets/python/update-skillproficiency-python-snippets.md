---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SkillProficiency()
request_body.setCategories(['Professional', ])

request_body.setProficiency(SkillProficiencyLevel('advancedprofessional'))


request_config = SkillProficiencyRequestBuilderPatchRequestConfiguration(
request_config = SkillProficiencyRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.me.profile.skills_by_id('skillProficiency-id').patch(request_body, headers=)


```