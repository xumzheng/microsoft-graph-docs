---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PersonCertification();
$requestBody->setCertificationId('KB-1235466333663322');

$requestBody->setDescription('Blackbelt in Marketing - Brand Management');

$requestBody->setDisplayName('Marketing Blackbelt - Brand Management');

$requestBody->setThumbnailUrl('https://iame.io/dfhdfdfd334.jpg');

$requestBody->setWebUrl('https://www.iame.io/blackbelt');



$requestResult = $graphServiceClient->me()->profile()->certifications()->post($requestBody);


```