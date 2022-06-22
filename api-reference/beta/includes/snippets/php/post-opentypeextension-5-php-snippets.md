---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Conversation();


$requestRequestBody->setTopic('Does anyone have a second?');
$threadsArray = [];

$threads1 = new ConversationThread();

$postsArray = [];

$posts1 = new Post();


$body = new ItemBody();
$posts1->setBody($body);


$body->setContentType(new BodyType('HTML'));
$body->setContent('This is urgent!');

$extensionsArray = [];

$extensions1 = new Extension();

$extensions1AdditionalData = [
			"@odata.type" => 'microsoft.graph.openTypeExtension',
			"extensionName" => 'Com.Contoso.Benefits',
			"companyName" => 'Contoso',
			"expirationDate" => '2016-08-03T11:00:00.000Z',
			"topPicks" =>  [
'Employees only','Add spouse or guest','Add family',			],
		];
$extensions1->setAdditionalData($extensions1AdditionalData);

$extensionsArray []= $extensions1;
$posts1->setExtensions($extensionsArray);

$postsArray []= $posts1;
$threads1->setPosts($postsArray);

$threadsArray []= $threads1;
$requestRequestBody->setThreads($threadsArray);
$result =  $graphClient->groupsById('group-id')->conversations()->post($requestRequestBody);


```