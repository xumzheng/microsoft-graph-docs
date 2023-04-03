---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ProjectParticipation();
requestBody.setCategories(['Branding', ]);

client = CompanyDetail();
client.setDisplayName('Contoso Ltd.');

client.setDepartment('Corporate Marketing');

client.setWebUrl('https://www.contoso.com');


requestBody.setClient($client);
requestBody.setDisplayName('Contoso Re-branding Project');

detail = PositionDetail();
detailCompany = CompanyDetail();
detailCompany.setDisplayName('Adventureworks Inc.');

detailCompany.setDepartment('Consulting');

detailCompany.setWebUrl('https://adventureworks.com');


detail.setCompany($detailCompany);
detail.setDescription('Rebranding of Contoso Ltd.');

detail.setJobTitle('Lead PM Rebranding');

detail.setRole('project management');

detail.setSummary('A 6 month project to help Contoso rebrand after they were divested from a parent organization.');


requestBody.setDetail($detail);


requestResult = graphServiceClient.me().profile().projects().post(requestBody);


```