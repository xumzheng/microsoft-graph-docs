---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PersonInterest()
request_body.setCategories(['Sports', ])

request_body.setDescription('World\'s greatest football club')

request_body.setDisplayName('Chelsea FC')

request_body.setWebUrl('https://www.chelseafc.com')



result = await client.me.profile.interests.post(request_body)


```