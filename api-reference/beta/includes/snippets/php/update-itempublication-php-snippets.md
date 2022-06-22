---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ItemPublication();


$requestRequestBody->setPublisher('International Association of Branding Management Publishing');
$requestRequestBody->setThumbnailUrl('https://iabm.io/sdhdfhsdhshsd.jpg');
$result =  $graphClient->usersById('user-id')->profile()->publicationsById('itemPublication-id')->patch($requestRequestBody);


```