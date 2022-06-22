---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TodoTask();


$requestRequestBody->setTitle('A new task');
$requestRequestBody->setCategories( [
'Important',],
$linkedResourcesArray = [];

$linkedResources1 = new LinkedResource();

$linkedResources1->setWebUrl('http://microsoft.com');
$linkedResources1->setApplicationName('Microsoft');
$linkedResources1->setDisplayName('Microsoft');

$linkedResourcesArray []= $linkedResources1;
$requestRequestBody->setLinkedResources($linkedResourcesArray);
$result =  $graphClient->me()->todo()->listsById('todoTaskList-id')->tasks()->post($requestRequestBody);


```