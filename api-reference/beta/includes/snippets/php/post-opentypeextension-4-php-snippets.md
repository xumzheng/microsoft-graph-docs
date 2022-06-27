---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PostRequestBody();



$post = new Post();
$requestRequestBody->setPost($post);



$body = new ItemBody();
$post->setBody($body);


$body->setContentType(new BodyType('html'));
$body->setContent('<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>');

$extensionsArray = [];

$extensionsextensions1 = new Extension();

$extensionsextensions1AdditionalData = [
"@odata.type" => 'microsoft.graph.openTypeExtension',
"extensionName" => 'Com.Contoso.HR',
"companyName" => 'Contoso',
"expirationDate" => '2015-07-03T13:04:00.000Z',
"topPicks" => ['Employees only','Add spouse or guest','Add family',],
];
$extensionsextensions1->setAdditionalData($extensionsextensions1AdditionalData);

$extensionsArray []= $extensionsextensions1;
$post->setExtensions($extensionsArray);

$result =  $graphClient->groupsById('group-id')->threadsById('conversationThread-id')->postsById('post-id')->reply()->post($requestRequestBody);


```