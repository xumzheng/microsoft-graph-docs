---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = SkillProficiency();
requestBody.setCategories(['Professional', ]);

requestBody.setProficiency(SkillProficiencyLevel('advancedprofessional'));



result = awaitclient.me().profile().skillsById('skillProficiency-id').patch(requestBody);


```