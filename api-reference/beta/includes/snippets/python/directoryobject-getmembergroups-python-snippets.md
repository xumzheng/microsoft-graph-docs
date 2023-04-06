---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetMemberGroupsPostRequestBody()
request_body.setSecurityEnabledOnly(false)


request_config = GetMemberGroupsRequestBuilderPostRequestConfiguration(
request_config = GetMemberGroupsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.directoryObjects_by_id('directoryObject-id').getMemberGroups.post(request_body, headers=)


```