---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AttributeSet();


$requestRequestBody->setId('Engineering');
$requestRequestBody->setDescription('Attributes for engineering team');
$requestRequestBody->setMaxAttributesPerSet(25);
$result =  $graphClient->directory()->attributeSets()->post($requestRequestBody);


```