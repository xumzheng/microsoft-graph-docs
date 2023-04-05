---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MessageRule()
request_body.setDisplayName('Important from partner')

actions = MessageRuleActions()
actions.setMarkImportance(Importance('high'))


request_body.setActions($actions)


result = await client.me.mailFolders._by_id('mailFolder-id').messageRules._by_id('messageRule-id').patch(request_body)


```