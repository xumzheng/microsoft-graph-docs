---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CheckinPostRequestBody();


$requestRequestBody->setComment('Updating the latest guidelines');
$result =  $graphClient->drivesById('drive-id')->itemsById('driveItem-id')->checkin()->post($requestRequestBody);


```