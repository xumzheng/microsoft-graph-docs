---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SetUpFeedbackResourcesFolderPostRequestBody();


requestResult = graphServiceClient.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').setUpFeedbackResourcesFolder().post(requestBody);


```