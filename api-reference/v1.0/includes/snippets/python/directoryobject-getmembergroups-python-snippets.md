---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = GetMemberGroupsPostRequestBody()
request_body.setSecurityEnabledOnly(false)



result = await client.directoryObjectsById('directoryObject-id').getMemberGroups.post(request_body)


```