---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SetUpFeedbackResourcesFolderPostRequestBody();


result = await client.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').setUpFeedbackResourcesFolder().post(requestBody);


```