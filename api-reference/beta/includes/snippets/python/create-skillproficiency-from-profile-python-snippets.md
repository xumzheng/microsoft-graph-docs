---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SkillProficiency();
requestBody.setCategories(['Professional', ]);

requestBody.setAllowedAudiences(AllowedAudiences('organization'));

requestBody.setDisplayName('API Design');

requestBody.setProficiency(SkillProficiencyLevel('generalprofessional'));

requestBody.setCollaborationTags(['ableToMentor', ]);



result = await client.me().profile().skills().post(requestBody);


```