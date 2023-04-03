---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = MessageRule();
requestBody.setDisplayName('From partner');

requestBody.setSequence(2);

requestBody.setIsEnabled(true);

conditions = MessageRulePredicates();
conditions.setSenderContains(['adele', ]);


requestBody.setConditions($conditions);
actions = MessageRuleActions();
forwardToRecipient1 = Recipient();
forwardToRecipient1EmailAddress = EmailAddress();
forwardToRecipient1EmailAddress.setName('Alex Wilbur');

forwardToRecipient1EmailAddress.setAddress('AlexW@contoso.onmicrosoft.com');


forwardToRecipient1.setEmailAddress($forwardToRecipient1EmailAddress);

forwardToArray []= forwardToRecipient1;
actions.setForwardTo(forwardToArray);


actions.setStopProcessingRules(true);


requestBody.setActions($actions);


result = await client.me().mailFoldersById('mailFolder-id').messageRules().post(requestBody);


```