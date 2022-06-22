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
$body->setContent('Hello World <at id="0">Jane Smith</at>');

$mentionsArray = [];

$mentions1 = new ChatMessageMention();

$mentions1->setId(0);
$mentions1->setMentionText('Jane Smith');

$mentioned = new ChatMessageMentionedIdentitySet();
$mentions1->setMentioned($mentioned);



$user = new Identity();
$mentioned->setUser($user);


$user->setDisplayName('Jane Smith');
$user->setId('ef1c916a-3135-4417-ba27-8eb7bd084193');
$userAdditionalData = [
	"userIdentityType" => 'aadUser',
];
$user->setAdditionalData($userAdditionalData);



$mentionsArray []= $mentions1;
$requestRequestBody->setMentions($mentionsArray);
$result =  $graphClient->teamsById('team-id')->channelsById('channel-id')->messages()->post($requestRequestBody);


```