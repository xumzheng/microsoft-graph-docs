---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationClass()
request_body.description = 'History - World History 1'

request_body.displayName = 'World History Level 1'



request_configuration = EducationClassRequestBuilderPatchRequestConfiguration(
)


result = await client.education.classes_by_id('educationClass-id').patch(request_body = request_body)


```