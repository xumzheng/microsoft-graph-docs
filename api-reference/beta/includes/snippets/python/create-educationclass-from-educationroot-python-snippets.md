---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = EducationClass()
request_body.setDescription('Health Level 1')

request_body.setClassCode('Health 501')

request_body.setDisplayName('Health 1')

request_body.setExternalId('11019')

request_body.setExternalName('Health Level 1')

request_body.setExternalSource(EducationExternalSource('sis'))

request_body.setMailNickname('fineartschool.net')



result = await client.education.classes.post(request_body)


```