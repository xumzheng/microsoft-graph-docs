---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MessageRule()
request_body.displayName = 'From partner'

request_body.sequence = 2

request_body.is_enabled = True

conditions = MessageRulePredicates()
conditions.SenderContains(['adele', ])


request_body.conditions = conditions
actions = MessageRuleActions()
forward_to_recipient1 = Recipient()
forward_to_recipient1_email_address = EmailAddress()
forwardToRecipient1EmailAddress.name = 'Alex Wilbur'

forwardToRecipient1EmailAddress.address = 'AlexW@contoso.onmicrosoft.com'


forwardToRecipient1.email_address = forwardToRecipient1EmailAddress

forwardToArray []= forwardToRecipient1;
actions.forwardto(forwardToArray)


actions.stop_processing_rules = True


request_body.actions = actions



result = await client.me.mailFolders_by_id('mailFolder-id').messageRules.post(request_body = request_body)


```