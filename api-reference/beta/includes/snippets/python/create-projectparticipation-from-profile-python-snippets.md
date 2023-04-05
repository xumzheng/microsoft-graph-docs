---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ProjectParticipation()
request_body.setCategories(['Branding', ])

client = CompanyDetail()
client.setDisplayName('Contoso Ltd.')

client.setDepartment('Corporate Marketing')

client.setWebUrl('https://www.contoso.com')


request_body.setClient($client)
request_body.setDisplayName('Contoso Re-branding Project')

detail = PositionDetail()
detailCompany = CompanyDetail()
detailCompany.setDisplayName('Adventureworks Inc.')

detailCompany.setDepartment('Consulting')

detailCompany.setWebUrl('https://adventureworks.com')


detail.setCompany($detailCompany)
detail.setDescription('Rebranding of Contoso Ltd.')

detail.setJobTitle('Lead PM Rebranding')

detail.setRole('project management')

detail.setSummary('A 6 month project to help Contoso rebrand after they were divested from a parent organization.')


request_body.setDetail($detail)


result = await client.me.profile.projects.post(request_body)


```