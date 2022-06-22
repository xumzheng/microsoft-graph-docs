---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new MessageRule();


$requestRequestBody->setDisplayName('Important from partner');

$actions = new MessageRuleActions();
$requestRequestBody->setActions($actions);


$actions->setMarkImportance(new Importance('high'));

$result =  $graphClient->me()->mailFoldersById('mailFolder-id')->messageRulesById('messageRule-id')->patch($requestRequestBody);


```