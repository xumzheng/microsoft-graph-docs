---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ProjectParticipation()
request_body.setAllowedAudiences(AllowedAudiences('organization'))

client = CompanyDetail()
client.setDepartment('Corporate Marketing')

client.setWebUrl('https://www.contoso.com')


request_body.setClient($client)


result = await client.me.profile.projectsById('projectParticipation-id').patch(request_body)


```