---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SkillProficiency();
requestBody.setCategories(['Professional', ]);

requestBody.setProficiency(SkillProficiencyLevel('advancedprofessional'));



result = await client.me().profile().skillsById('skillProficiency-id').patch(requestBody);


```