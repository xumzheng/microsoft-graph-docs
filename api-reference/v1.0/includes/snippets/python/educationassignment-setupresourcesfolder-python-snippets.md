---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SetUpResourcesFolderPostRequestBody();


requestResult = graphServiceClient.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').setUpResourcesFolder().post(requestBody);


```