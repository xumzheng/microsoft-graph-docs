---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new SkillProficiency();
$requestBody.setCategories(['Professional', ]);

$requestBody.setAllowedAudiences(new AllowedAudiences('organization'));

$requestBody.setDisplayName('API Design');

$requestBody.setProficiency(new SkillProficiencyLevel('generalprofessional'));

$requestBody.setCollaborationTags(['ableToMentor', ]);



$requestResult = $graphServiceClient.me().profile().skills().post($requestBody);


```