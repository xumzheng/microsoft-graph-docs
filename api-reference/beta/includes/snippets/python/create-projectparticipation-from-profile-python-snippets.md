---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ProjectParticipation()
request_body.Categories(['Branding', ])

client = CompanyDetail()
client.displayName = 'Contoso Ltd.'

client.department = 'Corporate Marketing'

client.webUrl = 'https://www.contoso.com'


request_body.client = client
request_body.displayName = 'Contoso Re-branding Project'

detail = PositionDetail()
detailCompany = CompanyDetail()
detailCompany.displayName = 'Adventureworks Inc.'

detailCompany.department = 'Consulting'

detailCompany.webUrl = 'https://adventureworks.com'


detail.company = detailCompany
detail.description = 'Rebranding of Contoso Ltd.'

detail.jobTitle = 'Lead PM Rebranding'

detail.role = 'project management'

detail.summary = 'A 6 month project to help Contoso rebrand after they were divested from a parent organization.'


request_body.detail = detail



result = await client.me.profile.projects.post(request_body = request_body)


```