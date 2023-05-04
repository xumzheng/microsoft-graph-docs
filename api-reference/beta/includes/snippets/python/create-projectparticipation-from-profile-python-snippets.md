---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Project_participation()
request_body.Categories(['Branding', ])

client = Company_detail()
client.display_name = 'Contoso Ltd.'

client.department = 'Corporate Marketing'

client.web_url = 'https://www.contoso.com'


request_body.client = client
request_body.display_name = 'Contoso Re-branding Project'

detail = Position_detail()
detailcompany = Company_detail()
detailcompany.display_name = 'Adventureworks Inc.'

detailcompany.department = 'Consulting'

detailcompany.web_url = 'https://adventureworks.com'


detail.company = detailcompany
detail.description = 'Rebranding of Contoso Ltd.'

detail.job_title = 'Lead PM Rebranding'

detail.role = 'project management'

detail.summary = 'A 6 month project to help Contoso rebrand after they were divested from a parent organization.'


request_body.detail = detail



result = await client.me.profile.projects.post(request_body = request_body)


```