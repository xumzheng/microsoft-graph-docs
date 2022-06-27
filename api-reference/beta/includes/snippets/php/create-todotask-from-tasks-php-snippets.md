---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TodoTask();


$requestRequestBody->setTitle('A new task');
$requestRequestBody->setCategories(['Important',]);
$linkedResourcesArray = [];

$linkedResourceslinkedResources1 = new LinkedResource();

$linkedResourceslinkedResources1->setWebUrl('http://microsoft.com');
$linkedResourceslinkedResources1->setApplicationName('Microsoft');
$linkedResourceslinkedResources1->setDisplayName('Microsoft');

$linkedResourcesArray []= $linkedResourceslinkedResources1;
$requestRequestBody->setLinkedResources($linkedResourcesArray);
$result =  $graphClient->me()->todo()->listsById('todoTaskList-id')->tasks()->post($requestRequestBody);


```