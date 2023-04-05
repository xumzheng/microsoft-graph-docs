---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationSchool()
request_body.setDisplayName('Fabrikam High School')

request_body.setDescription('Magnate school for the arts. Los Angeles School District')

request_body.setExternalSource(EducationExternalSource('string'))

request_body.setPrincipalEmail('AmyR@fabrikam.com')

request_body.setPrincipalName('Amy Roebuck')

request_body.setExternalPrincipalId('14007')

request_body.setHighestGrade('12')

request_body.setLowestGrade('9')

request_body.setSchoolNumber('10002')

address = PhysicalAddress()
address.setCity('Los Angeles')

address.setCountryOrRegion('United States')

address.setPostalCode('98055')

address.setState('CA')

address.setStreet('12345 Main St.')


request_body.setAddress($address)
request_body.setExternalId('10002')

request_body.setPhone('+1 (253) 555-0102')



result = await client.education_schools.post(request_body)


```