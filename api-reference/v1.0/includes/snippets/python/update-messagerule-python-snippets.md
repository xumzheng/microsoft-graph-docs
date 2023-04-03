---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = MessageRule();
requestBody.setDisplayName('Important from partner');

actions = MessageRuleActions();
actions.setMarkImportance(Importance('high'));


requestBody.setActions($actions);


requestResult = graphServiceClient.me().mailFoldersById('mailFolder-id').messageRulesById('messageRule-id').patch(requestBody);


```