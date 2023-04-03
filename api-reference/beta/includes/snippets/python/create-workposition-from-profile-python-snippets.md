---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = WorkPosition();
detail = PositionDetail();
detailCompany = CompanyDetail();
detailCompany.setDisplayName('Adventureworks Ltd.');

detailCompany.setDepartment('Consulting');

detailCompany.setOfficeLocation('AW23/344');

detailCompanyAddress = PhysicalAddress();
detailCompanyAddress.setType(PhysicalAddressType('business'));

detailCompanyAddress.setStreet('123 Patriachy Ponds');

detailCompanyAddress.setCity('Moscow');

detailCompanyAddress.setCountryOrRegion('Russian Federation');

detailCompanyAddress.setPostalCode('RU-34621');


detailCompany.setAddress($detailCompanyAddress);
detailCompany.setWebUrl('https://www.adventureworks.com');


detail.setCompany($detailCompany);
detail.setJobTitle('Senior Product Branding Manager II');

detail.setRole('consulting');


requestBody.setDetail($detail);
requestBody.setIsCurrent(true);



requestResult = graphServiceClient.me().profile().positions().post(requestBody);


```