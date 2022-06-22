---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CustomSecurityAttributeDefinition();


$requestRequestBody->setStatus('Deprecated');
$result =  $graphClient->directory()->customSecurityAttributeDefinitionsById('customSecurityAttributeDefinition-id')->patch($requestRequestBody);


```