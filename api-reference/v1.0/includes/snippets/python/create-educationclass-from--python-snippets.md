---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationClass()
request_body.@odatatype = '#microsoft.graph.educationClass'

request_body.displayName = 'String'

request_body.mailNickname = 'String'

request_body.description = 'String'

createdBy = IdentitySet()
createdBy.@odatatype = 'microsoft.graph.identitySet'


request_body.createdBy = createdBy
request_body.classCode = 'String'

request_body.externalName = 'String'

request_body.externalId = 'String'

request_body.ExternalSource(EducationExternalSource('string'))

request_body.externalSourceDetail = 'String'

request_body.grade = 'String'

term = EducationTerm()
term.@odatatype = 'microsoft.graph.educationTerm'


request_body.term = term


request_configuration = ClassesRequestBuilderPostRequestConfiguration(
)


result = await client.education.classes.post(request_body = request_body)


```