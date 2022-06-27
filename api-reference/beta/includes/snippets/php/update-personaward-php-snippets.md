---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PersonAward();


$requestRequestBody->setIssuingAuthority('International Association of Branding Management');
$requestRequestBody->setThumbnailUrl('https://iabm.io/sdhdfhsdhshsd.jpg');
$result =  $graphClient->usersById('user-id')->profile()->awardsById('personAward-id')->patch($requestRequestBody);


```