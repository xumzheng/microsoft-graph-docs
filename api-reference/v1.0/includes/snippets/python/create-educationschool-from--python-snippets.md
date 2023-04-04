---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = EducationSchool()
request_body.set@odatatype('#microsoft.graph.educationSchool')

request_body.setDisplayName('String')

request_body.setDescription('String')

request_body.setExternalSource(EducationExternalSource('string'))

request_body.setExternalSourceDetail('String')

request_body.setPrincipalEmail('String')

request_body.setPrincipalName('String')

request_body.setExternalPrincipalId('String')

request_body.setLowestGrade('String')

request_body.setHighestGrade('String')

request_body.setSchoolNumber('String')

request_body.setExternalId('String')

request_body.setPhone('String')

request_body.setFax('String')

createdBy = IdentitySet()
createdBy.set@odatatype('microsoft.graph.identitySet')


request_body.setCreatedBy($createdBy)
address = PhysicalAddress()
address.set@odatatype('microsoft.graph.physicalAddress')


request_body.setAddress($address)


result = await client.education.schools.post(request_body)


```