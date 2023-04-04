---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = SkillProficiency();
request_body.setCategories(['Professional', ]);

request_body.setAllowedAudiences(AllowedAudiences('organization'));

request_body.setDisplayName('API Design');

request_body.setProficiency(SkillProficiencyLevel('generalprofessional'));

request_body.setCollaborationTags(['ableToMentor', ]);



result = await client.me().profile().skills().post(request_body);


```