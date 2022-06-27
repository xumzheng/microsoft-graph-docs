---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CustomSecurityAttributeDefinition();


$requestRequestBody->setAttributeSet('Engineering');
$requestRequestBody->setDescription('Target completion date');
$requestRequestBody->setIsCollection(False);
$requestRequestBody->setIsSearchable(True);
$requestRequestBody->setName('ProjectDate');
$requestRequestBody->setStatus('Available');
$requestRequestBody->setType('String');
$requestRequestBody->setUsePreDefinedValuesOnly(False);
$result =  $graphClient->directory()->customSecurityAttributeDefinitions()->post($requestRequestBody);


```