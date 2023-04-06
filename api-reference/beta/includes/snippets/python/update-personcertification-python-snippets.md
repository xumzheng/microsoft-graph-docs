---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PersonCertification()
request_body.setIssuingAuthority('International Academy of Marketing Excellence')

request_body.setIssuingCompany('International Academy of Marketing Excellence')



result = await client.users_by_id('user-id').profile.certifications_by_id('personCertification-id').patch(request_body, headers=)


```