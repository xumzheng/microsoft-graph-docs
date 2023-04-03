---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SkillProficiency();
requestBody.setCategories(['Professional', ]);

requestBody.setProficiency(SkillProficiencyLevel('advancedprofessional'));



requestResult = graphServiceClient.me().profile().skillsById('skillProficiency-id').patch(requestBody);


```