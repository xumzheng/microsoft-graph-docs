---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Channel();
$requestBody->setDisplayName('Architecture Discussion');

$requestBody->setDescription('This channel is where we debate all future architecture plans');

$requestBody->setMembershipType(new ChannelMembershipType('standard'));



$requestResult = $graphServiceClient->teamsById('team-id')->channels()->post($requestBody);


```