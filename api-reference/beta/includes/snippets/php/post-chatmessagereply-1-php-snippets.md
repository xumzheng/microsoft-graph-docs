---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ChatMessage();



$body = new ItemBody();
$requestRequestBody->setBody($body);


$body->setContentType(new BodyType('html'));
$body->setContent('Hello World');

$result =  $graphClient->teamsById('team-id')->channelsById('channel-id')->messagesById('chatMessage-id')->replies()->post($requestRequestBody);


```