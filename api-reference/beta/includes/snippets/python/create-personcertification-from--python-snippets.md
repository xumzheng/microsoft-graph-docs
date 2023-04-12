---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PersonCertification()
request_body.certificationId = 'KB-1235466333663322'

request_body.description = 'Blackbelt in Marketing - Brand Management'

request_body.displayName = 'Marketing Blackbelt - Brand Management'

request_body.thumbnailUrl = 'https://iame.io/dfhdfdfd334.jpg'

request_body.webUrl = 'https://www.iame.io/blackbelt'




result = await client.me.profile.certifications.post(request_body = request_body)


```