---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ItemPublication();


$requestRequestBody->setDescription('One persons journey to the top of the branding management field.');
$requestRequestBody->setDisplayName('Got Brands? The story of Innocenty Popov and his journey to the top.');
$requestRequestBody->setPublishedDate('Date');
$requestRequestBody->setPublisher('International Association of Branding Management Publishing');
$requestRequestBody->setThumbnailUrl('https://iabm.io/sdhdfhsdhshsd.jpg');
$requestRequestBody->setWebUrl('https://www.iabm.io');
$result =  $graphClient->me()->profile()->publications()->post($requestRequestBody);


```