---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationClass()
request_body.set@odatatype('#microsoft.graph.educationClass')

request_body.setDisplayName('String')

request_body.setMailNickname('String')

request_body.setDescription('String')

createdBy = IdentitySet()
createdBy.set@odatatype('microsoft.graph.identitySet')


request_body.setCreatedBy($createdBy)
request_body.setClassCode('String')

request_body.setExternalName('String')

request_body.setExternalId('String')

request_body.setExternalSource(EducationExternalSource('string'))

request_body.setExternalSourceDetail('String')

request_body.setGrade('String')

term = EducationTerm()
term.set@odatatype('microsoft.graph.educationTerm')


request_body.setTerm($term)


result = await client.education.classes.post(request_body, headers=)


```