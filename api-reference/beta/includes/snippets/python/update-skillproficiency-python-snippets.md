---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new SkillProficiency();
$requestBody.setCategories(['Professional', ]);

$requestBody.setProficiency(new SkillProficiencyLevel('advancedprofessional'));



$requestResult = $graphServiceClient.me().profile().skillsById('skillProficiency-id').patch($requestBody);


```