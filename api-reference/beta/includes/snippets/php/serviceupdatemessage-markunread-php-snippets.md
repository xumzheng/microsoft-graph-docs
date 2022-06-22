---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new MessageIdsRequestBody();


$requestRequestBody->setMessageIds( [
'MC172851','MC167983',],
$result =  $graphClient->admin()->serviceAnnouncement()->messages()->markUnread()->post($requestRequestBody);


```