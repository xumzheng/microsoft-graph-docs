---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Conversation();


$requestRequestBody->setTopic('Does anyone have a second?');
$threadsArray = [];

$threadsthreads1 = new ConversationThread();

$postsArray = [];

$postsposts1 = new Post();


$body = new ItemBody();
$postsposts1->setBody($body);


$body->setContentType(new BodyType('HTML'));
$body->setContent('This is urgent!');

$extensionsArray = [];

$extensionsextensions1 = new Extension();

$extensionsextensions1AdditionalData = [
"@odata.type" => 'microsoft.graph.openTypeExtension',
"extensionName" => 'Com.Contoso.Benefits',
"companyName" => 'Contoso',
"expirationDate" => '2016-08-03T11:00:00.000Z',
"topPicks" => ['Employees only','Add spouse or guest','Add family',],
];
$extensionsextensions1->setAdditionalData($extensionsextensions1AdditionalData);

$extensionsArray []= $extensionsextensions1;
$postsposts1->setExtensions($extensionsArray);

$postsArray []= $postsposts1;
$threadsthreads1->setPosts($postsArray);

$threadsArray []= $threadsthreads1;
$requestRequestBody->setThreads($threadsArray);
$result =  $graphClient->groupsById('group-id')->conversations()->post($requestRequestBody);


```