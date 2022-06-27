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
$body->setContent('<div><div><at id="0">TestTag</at>&nbsp;Testing Tags</div></div>');

$mentionsArray = [];

$mentionsmentions1 = new ChatMessageMention();

$mentionsmentions1->setId(0);
$mentionsmentions1->setMentionText('TestTag');

$mentioned = new ChatMessageMentionedIdentitySet();
$mentionsmentions1->setMentioned($mentioned);



$tag = new TeamworkTagIdentity();
$mentioned->setTag($tag);


$tag->setId('MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM2OGEzZTM2NS1mN2Q5LTRhNTYtYjQ5OS0yNDMzMmE5Y2M1NzIjI3RTMERJZ1Z1ZQ==');
$tag->setDisplayName('TestTag');



$mentionsArray []= $mentionsmentions1;
$requestRequestBody->setMentions($mentionsArray);
$result =  $graphClient->teamsById('team-id')->channelsById('channel-id')->messages()->post($requestRequestBody);


```