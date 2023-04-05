---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationClass()
request_body.setDescription('History - World History 1')

request_body.setDisplayName('World History Level 1')



result = await client.education.classesby_id('educationClass-id').patch(request_body)


```