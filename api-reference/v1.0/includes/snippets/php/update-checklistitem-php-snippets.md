---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ChecklistItem();


$requestRequestBody->setDisplayName('buy cake');
$result =  $graphClient->me()->todo()->listsById('todoTaskList-id')->tasksById('todoTask-id')->checklistItemsById('checklistItem-id')->patch($requestRequestBody);


```