---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MessageRule()
request_body.displayName = 'Important from partner'

actions = MessageRuleActions()
actions.MarkImportance(Importance('high'))


request_body.actions = actions


request_configuration = MessageRuleRequestBuilderPatchRequestConfiguration(
)


result = await client.me.mailFolders_by_id('mailFolder-id').messageRules_by_id('messageRule-id').patch(request_body = request_body)


```