---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationalActivity()
institution = InstitutionData()
institutionLocation = PhysicalAddress()
institutionLocation.setType(PhysicalAddressType('business'))

InstitutionLocation.setPostOfficeBox(null)

institutionLocation.setStreet('12000 E Prospect Rd')

institutionLocation.setCity('Fort Collins')

institutionLocation.setState('Colorado')

institutionLocation.setCountryOrRegion('USA')

institutionLocation.setPostalCode('80525')


institution.setLocation($institutionLocation)

request_body.setInstitution($institution)


result = await client.me.profile.educationalActivitiesById('educationalActivity-id').patch(request_body)


```