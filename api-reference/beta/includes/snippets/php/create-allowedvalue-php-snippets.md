---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AllowedValue();


$requestRequestBody->setId('Alpine');
$requestRequestBody->setIsActive('true');
$result =  $graphClient->directory()->customSecurityAttributeDefinitionsById('customSecurityAttributeDefinition-id')->allowedValues()->post($requestRequestBody);


```