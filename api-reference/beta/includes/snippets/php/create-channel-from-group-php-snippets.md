---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Channel();


$requestRequestBody->setDisplayName('Architecture Discussion');
$requestRequestBody->setDescription('This channel is where we debate all future architecture plans');
$requestRequestBody->setMembershipType(new ChannelMembershipType('standard'));
$result =  $graphClient->teamsById('team-id')->channels()->post($requestRequestBody);


```