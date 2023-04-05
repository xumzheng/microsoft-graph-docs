---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SetUpResourcesFolderPostRequestBody()


result = await client.education.classesby_id('educationClass-id').assignmentsby_id('educationAssignment-id').setUpResourcesFolder.post(request_body)


```