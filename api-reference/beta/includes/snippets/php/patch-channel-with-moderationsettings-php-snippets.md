---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Channel();


$requestRequestBody->setDisplayName('UpdateChannelModeration');
$requestRequestBody->setDescription('Update channel moderation.');

$moderationSettings = new ChannelModerationSettings();
$requestRequestBody->setModerationSettings($moderationSettings);


$moderationSettings->setUserNewMessageRestriction(new UserNewMessageRestriction('moderators'));
$moderationSettings->setReplyRestriction(new ReplyRestriction('everyone'));
$moderationSettings->setAllowNewMessageFromBots(True);
$moderationSettings->setAllowNewMessageFromConnectors(True);

$result =  $graphClient->teamsById('team-id')->channelsById('channel-id')->patch($requestRequestBody);


```