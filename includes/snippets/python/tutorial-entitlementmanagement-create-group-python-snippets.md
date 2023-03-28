---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Group();
$requestBody->setDescription('Marketing group');

$requestBody->setDisplayName('Marketing resources');

$requestBody->setMailEnabled(false);

$requestBody->setMailNickname('markres');

$requestBody->setSecurityEnabled(true);



$requestResult = $graphServiceClient->groups()->post($requestBody);


```