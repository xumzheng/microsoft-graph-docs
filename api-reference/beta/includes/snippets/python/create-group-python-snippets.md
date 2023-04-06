---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Group()
request_body.setDescription('Self help community for golf')

request_body.setDisplayName('Golf Assist')

request_body.setGroupTypes(['Unified', ])

request_body.setMailEnabled(true)

request_body.setMailNickname('golfassist')

request_body.setSecurityEnabled(false)


request_config = GroupsRequestBuilderPostRequestConfiguration(
request_config = GroupsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.groups.post(request_body, headers=)


```