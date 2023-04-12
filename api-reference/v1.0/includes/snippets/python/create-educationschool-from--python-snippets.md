---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationSchool()
request_body.@odatatype = '#microsoft.graph.educationSchool'

request_body.displayName = 'String'

request_body.description = 'String'

request_body.ExternalSource(EducationExternalSource('string'))

request_body.externalSourceDetail = 'String'

request_body.principalEmail = 'String'

request_body.principalName = 'String'

request_body.externalPrincipalId = 'String'

request_body.lowestGrade = 'String'

request_body.highestGrade = 'String'

request_body.schoolNumber = 'String'

request_body.externalId = 'String'

request_body.phone = 'String'

request_body.fax = 'String'

createdBy = IdentitySet()
createdBy.@odatatype = 'microsoft.graph.identitySet'


request_body.createdBy = createdBy
address = PhysicalAddress()
address.@odatatype = 'microsoft.graph.physicalAddress'


request_body.address = address



result = await client.education.schools.post(request_body = request_body)


```