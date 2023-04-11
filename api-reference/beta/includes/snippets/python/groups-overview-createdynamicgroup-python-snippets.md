---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Group()
request_body.description = 'Marketing department folks'

request_body.displayName = 'Marketing department'

request_body.GroupTypes(['Unified', 'DynamicMembership', ])

request_body.mailEnabled = true

request_body.mailNickname = 'marketing'

request_body.securityEnabled = false

request_body.membershipRule = 'user.department -eq \"Marketing\"'

request_body.membershipRuleProcessingState = 'on'



request_configuration = GroupsRequestBuilderPostRequestConfiguration(
)


result = await client.groups.post(request_body = request_body)


```