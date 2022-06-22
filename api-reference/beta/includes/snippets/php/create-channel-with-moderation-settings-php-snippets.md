---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Channel();


$requestRequestBody->setDisplayName('TestChannelModeration');
$requestRequestBody->setDescription('Test channel moderation.');
$requestRequestBody->setMembershipType(new ChannelMembershipType('standard'));

$moderationSettings = new ChannelModerationSettings();
$requestRequestBody->setModerationSettings($moderationSettings);


$moderationSettings->setUserNewMessageRestriction(new UserNewMessageRestriction('everyoneExceptGuests'));
$moderationSettings->setReplyRestriction(new ReplyRestriction('everyone'));
$moderationSettings->setAllowNewMessageFromBots(True);
$moderationSettings->setAllowNewMessageFromConnectors(True);

$result =  $graphClient->teamsById('team-id')->channels()->post($requestRequestBody);


```