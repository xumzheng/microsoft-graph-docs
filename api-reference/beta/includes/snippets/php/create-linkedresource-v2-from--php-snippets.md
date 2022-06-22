---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new LinkedResource_v2();


$requestRequestBody->setWebUrl('https://microsoft.com');
$requestRequestBody->setApplicationName('Microsoft');
$requestRequestBody->setDisplayName('Microsoft');
$requestRequestBody->setExternalId('dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9');
$result =  $graphClient->me()->tasks()->listsById('baseTaskList-id')->tasksById('baseTask-id')->linkedResources()->post($requestRequestBody);


```