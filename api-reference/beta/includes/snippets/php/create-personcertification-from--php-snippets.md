---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PersonCertification();


$requestRequestBody->setCertificationId('KB-1235466333663322');
$requestRequestBody->setDescription('Blackbelt in Marketing - Brand Management');
$requestRequestBody->setDisplayName('Marketing Blackbelt - Brand Management');
$requestRequestBody->setThumbnailUrl('https://iame.io/dfhdfdfd334.jpg');
$requestRequestBody->setWebUrl('https://www.iame.io/blackbelt');
$result =  $graphClient->me()->profile()->certifications()->post($requestRequestBody);


```