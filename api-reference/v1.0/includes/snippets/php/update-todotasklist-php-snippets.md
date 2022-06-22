---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TodoTaskList();


$requestRequestBody->setDisplayName('Vacation Plan');
$result =  $graphClient->me()->todo()->listsById('todoTaskList-id')->patch($requestRequestBody);


```