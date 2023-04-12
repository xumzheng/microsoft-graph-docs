---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationUser()
request_body.displayName = 'Rogelio Cazares'

request_body.givenName = 'Rogelio'

request_body.middleName = 'Fernando'

request_body.surname = 'Cazares'




result = await client.education.users_by_id('educationUser-id').patch(request_body = request_body)


```