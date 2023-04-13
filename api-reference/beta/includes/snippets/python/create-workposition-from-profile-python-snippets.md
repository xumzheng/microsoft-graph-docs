---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = WorkPosition()
detail = PositionDetail()
detailCompany = CompanyDetail()
detailCompany.displayName = 'Adventureworks Ltd.'

detailCompany.department = 'Consulting'

detailCompany.officeLocation = 'AW23/344'

detailCompanyAddress = PhysicalAddress()
detailCompanyAddress.Type(PhysicalAddressType('business'))

detailCompanyAddress.street = '123 Patriachy Ponds'

detailCompanyAddress.city = 'Moscow'

detailCompanyAddress.countryOrRegion = 'Russian Federation'

detailCompanyAddress.postalCode = 'RU-34621'


detailCompany.address = detailCompanyAddress
detailCompany.webUrl = 'https://www.adventureworks.com'


detail.company = detailCompany
detail.jobTitle = 'Senior Product Branding Manager II'

detail.role = 'consulting'


request_body.detail = detail
request_body.isCurrent = true




result = await client.me.profile.positions.post(request_body = request_body)


```