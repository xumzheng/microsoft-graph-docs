---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ReferenceUpdate();
$requestBody.set@odataid('https://graph.microsoft.com/v1.0/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d');



$graphServiceClient.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').rubric().ref().put($requestBody);


```