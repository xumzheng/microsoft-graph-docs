---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PersonCertification()
request_body.setCertificationId('KB-1235466333663322')

request_body.setDescription('Blackbelt in Marketing - Brand Management')

request_body.setDisplayName('Marketing Blackbelt - Brand Management')

request_body.setThumbnailUrl('https://iame.io/dfhdfdfd334.jpg')

request_body.setWebUrl('https://www.iame.io/blackbelt')



result = await client.me.profile.certifications.post(request_body)


```