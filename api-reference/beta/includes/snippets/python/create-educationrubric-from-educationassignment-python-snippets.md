---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceUpdate()
request_body.set@odataid('https://graph.microsoft.com/v1.0/education/me/rubrics/{id}')



await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').rubric.ref.put(request_body)


```