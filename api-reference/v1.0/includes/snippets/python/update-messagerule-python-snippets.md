---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = MessageRule();
requestBody.setDisplayName('Important from partner');

actions = MessageRuleActions();
actions.setMarkImportance(Importance('high'));


requestBody.setActions($actions);


result = await client.me().mailFoldersById('mailFolder-id').messageRulesById('messageRule-id').patch(requestBody);


```