---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = SkillProficiency();
requestBody.setCategories(['Professional', ]);

requestBody.setAllowedAudiences(AllowedAudiences('organization'));

requestBody.setDisplayName('API Design');

requestBody.setProficiency(SkillProficiencyLevel('generalprofessional'));

requestBody.setCollaborationTags(['ableToMentor', ]);



result = awaitclient.me().profile().skills().post(requestBody);


```