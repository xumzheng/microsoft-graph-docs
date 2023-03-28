---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new MessageRule();
$requestBody->setDisplayName('Important from partner');

$actions = new MessageRuleActions();
$actions->setMarkImportance(new Importance('high'));


$requestBody->setActions($actions);


$requestResult = $graphServiceClient->me()->mailFoldersById('mailFolder-id')->messageRulesById('messageRule-id')->patch($requestBody);


```