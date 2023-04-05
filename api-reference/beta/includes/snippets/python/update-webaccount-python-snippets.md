---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = WebAccount()
request_body.setWebUrl('https://github.com/innocenty.popov')



result = await client.me.profile.webAccountsById('webAccount-id').patch(request_body)


```