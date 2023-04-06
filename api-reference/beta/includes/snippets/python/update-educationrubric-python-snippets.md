---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationRubric()
request_body.setDisplayName('Example Credit Rubric after display name patch')


request_config = EducationRubricRequestBuilderPatchRequestConfiguration(
request_config = EducationRubricRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.education.me.rubrics_by_id('educationRubric-id').patch(request_body, headers=)


```