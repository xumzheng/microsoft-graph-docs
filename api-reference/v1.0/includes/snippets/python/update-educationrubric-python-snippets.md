---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new EducationRubric();
$requestBody->setDisplayName('Example Credit Rubric after display name patch');



$requestResult = $graphServiceClient->education()->me()->rubricsById('educationRubric-id')->patch($requestBody);


```