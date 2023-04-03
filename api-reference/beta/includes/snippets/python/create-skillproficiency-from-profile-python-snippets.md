---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SkillProficiency();
requestBody.setCategories(['Professional', ]);

requestBody.setAllowedAudiences(AllowedAudiences('organization'));

requestBody.setDisplayName('API Design');

requestBody.setProficiency(SkillProficiencyLevel('generalprofessional'));

requestBody.setCollaborationTags(['ableToMentor', ]);



requestResult = graphServiceClient.me().profile().skills().post(requestBody);


```