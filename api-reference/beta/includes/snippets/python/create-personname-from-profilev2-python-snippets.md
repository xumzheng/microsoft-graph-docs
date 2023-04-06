---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PersonName()
request_body.setDisplayName('Innocenty Popov')

request_body.setFirst('Innocenty')

request_body.setInitials('IP')

request_body.setLast('Popov')

request_body.setLanguageTag('en-US')

request_body.setMaiden(null)



result = await client.me.profile.names.post(request_body, headers=)


```