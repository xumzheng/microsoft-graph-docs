---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DestinationTaskListIdRequestBody();


$requestRequestBody->setDestinationTaskListId('AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQqFxG');
$result =  $graphClient->me()->tasks()->listsById('baseTaskList-id')->tasksById('baseTask-id')->move()->post($requestRequestBody);


```