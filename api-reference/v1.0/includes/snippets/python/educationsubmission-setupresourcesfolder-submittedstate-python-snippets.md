---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SetUpResourcesFolderPostRequestBody()


result = await client.education.classesById('educationClass-id').assignmentsById('educationAssignment-id').submissionsById('educationSubmission-id').setUpResourcesFolder.post(request_body)


```