---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PersonAward()
request_body.issuingAuthority = 'International Association of Branding Management'

request_body.thumbnailUrl = 'https://iabm.io/sdhdfhsdhshsd.jpg'



request_configuration = PersonAwardRequestBuilderPatchRequestConfiguration(
)


result = await client.users_by_id('user-id').profile.awards_by_id('personAward-id').patch(request_body = request_body)


```