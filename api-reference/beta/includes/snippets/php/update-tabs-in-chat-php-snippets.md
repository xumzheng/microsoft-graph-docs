---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TeamsTab();


$requestRequestBody->setDisplayName('My Contoso Tab - updated again');
$result =  $graphClient->chatsById('chat-id')->tabsById('teamsTab-id')->patch($requestRequestBody);


```