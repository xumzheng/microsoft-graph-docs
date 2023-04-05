---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationSchool()
request_body.setDisplayName('Fabrikam Arts High School')

request_body.setDescription('Magnate school for the arts. Los Angeles School District')



result = await client.education.schoolsById('educationSchool-id').patch(request_body)


```