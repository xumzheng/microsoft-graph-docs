---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AttributeSet();


$requestRequestBody->setDescription('Attributes for engineering team');
$requestRequestBody->setMaxAttributesPerSet(20);
$result =  $graphClient->directory()->attributeSetsById('attributeSet-id')->patch($requestRequestBody);


```