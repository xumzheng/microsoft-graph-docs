---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TodoTaskList();


$requestRequestBody->setDisplayName('Travel items');
$result =  $graphClient->me()->todo()->lists()->post($requestRequestBody);


```