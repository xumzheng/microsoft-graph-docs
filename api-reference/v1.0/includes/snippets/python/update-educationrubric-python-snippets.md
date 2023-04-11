---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationRubric()
request_body.displayName = 'Example Credit Rubric after display name patch'



request_configuration = EducationRubricRequestBuilderPatchRequestConfiguration(
)


result = await client.education.me.rubrics_by_id('educationRubric-id').patch(request_body = request_body)


```