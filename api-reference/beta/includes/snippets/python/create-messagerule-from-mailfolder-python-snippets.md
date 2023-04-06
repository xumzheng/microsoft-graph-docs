---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MessageRule()
request_body.setDisplayName('From partner')

request_body.setSequence(2)

request_body.setIsEnabled(true)

conditions = MessageRulePredicates()
conditions.setSenderContains(['adele', ])


request_body.setConditions($conditions)
actions = MessageRuleActions()
forwardToRecipient1 = Recipient()
forwardToRecipient1EmailAddress = EmailAddress()
forwardToRecipient1EmailAddress.setName('Alex Wilbur')

forwardToRecipient1EmailAddress.setAddress('AlexW@contoso.onmicrosoft.com')


forwardToRecipient1.setEmailAddress($forwardToRecipient1EmailAddress)

forwardToArray []= forwardToRecipient1;
actions.setForwardTo(forwardToArray)


actions.setStopProcessingRules(true)


request_body.setActions($actions)


result = await client.me.mailFolders_by_id('mailFolder-id').messageRules.post(request_body, headers=)


```