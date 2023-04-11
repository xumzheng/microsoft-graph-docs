---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PersonCertification()
request_body.issuingAuthority = 'International Academy of Marketing Excellence'

request_body.issuingCompany = 'International Academy of Marketing Excellence'



request_configuration = PersonCertificationRequestBuilderPatchRequestConfiguration(
)


result = await client.users_by_id('user-id').profile.certifications_by_id('personCertification-id').patch(request_body = request_body)


```