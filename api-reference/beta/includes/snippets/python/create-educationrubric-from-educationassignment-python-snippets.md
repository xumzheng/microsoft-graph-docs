---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ReferenceUpdate();
requestBody.set@odataid('https://graph.microsoft.com/v1.0/education/me/rubrics/{id}');



await client.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').rubric().ref().put(requestBody);


```