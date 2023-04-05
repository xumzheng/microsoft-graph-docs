---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetMemberGroupsPostRequestBody()
request_body.setSecurityEnabledOnly(false)



result = await client.directoryObjectsby_id('directoryObject-id')_getMemberGroups.post(request_body)


```