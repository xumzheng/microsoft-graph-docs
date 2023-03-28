---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ChatMessage();
$body = new ItemBody();
$body->setContent('Hello World');


$requestBody->setBody($body);


$requestResult = $graphServiceClient->teamsById('team-id')->channelsById('channel-id')->messages()->post($requestBody);


```