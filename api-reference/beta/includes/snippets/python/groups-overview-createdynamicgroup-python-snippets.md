---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Group();
$requestBody->setDescription('Marketing department folks');

$requestBody->setDisplayName('Marketing department');

$requestBody->setGroupTypes(['Unified', 'DynamicMembership', ]);

$requestBody->setMailEnabled(true);

$requestBody->setMailNickname('marketing');

$requestBody->setSecurityEnabled(false);

$requestBody->setMembershipRule('user.department -eq \"Marketing\"');

$requestBody->setMembershipRuleProcessingState('on');



$requestResult = $graphServiceClient->groups()->post($requestBody);


```