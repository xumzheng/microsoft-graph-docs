---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceUpdate()
request_body.set@odataid('https://graph.microsoft.com/v1.0/education/me/rubrics/{id}')



await client.education_classesby_id('educationClass-id')_assignmentsby_id('educationAssignment-id')_rubric_ref.put(request_body)


```