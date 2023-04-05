---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Group()
request_body.setDescription('Marketing group')

request_body.setDisplayName('Marketing resources')

request_body.setMailEnabled(false)

request_body.setMailNickname('markres')

request_body.setSecurityEnabled(true)



result = await client.groups.post(request_body)


```