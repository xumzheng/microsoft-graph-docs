---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ItemAddress()
request_body.AllowedAudiences(AllowedAudiences('me'))

request_body.displayName = 'Secret Hideout'




result = await client.users_by_id('user-id').profile.addresses_by_id('itemAddress-id').patch(request_body = request_body)


```