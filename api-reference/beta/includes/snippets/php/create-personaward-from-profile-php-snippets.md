---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PersonAward();


$requestRequestBody->setDescription('Lifetime Achievement award from the International Association of Branding Managers');
$requestRequestBody->setDisplayName('Lifetime Achievement Award For Excellence in Branding');
$requestRequestBody->setIssuedDate('Date');
$requestRequestBody->setIssuingAuthority('International Association of Branding Management');
$requestRequestBody->setThumbnailUrl('https://iabm.io/sdhdfhsdhshsd.jpg');
$requestRequestBody->setWebUrl('https://www.iabm.io');
$result =  $graphClient->me()->profile()->awards()->post($requestRequestBody);


```