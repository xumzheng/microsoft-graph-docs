---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationSchool()
request_body.displayName = 'Fabrikam High School'

request_body.description = 'Magnate school for the arts. Los Angeles School District'

request_body.ExternalSource(EducationExternalSource('string'))

request_body.principalEmail = 'AmyR@fabrikam.com'

request_body.principalName = 'Amy Roebuck'

request_body.externalPrincipalId = '14007'

request_body.highestGrade = '12'

request_body.lowestGrade = '9'

request_body.schoolNumber = '10002'

address = PhysicalAddress()
address.city = 'Los Angeles'

address.countryOrRegion = 'United States'

address.postalCode = '98055'

address.state = 'CA'

address.street = '12345 Main St.'


request_body.address = address
request_body.externalId = '10002'

request_body.phone = '+1 (253) 555-0102'




result = await client.education.schools.post(request_body = request_body)


```