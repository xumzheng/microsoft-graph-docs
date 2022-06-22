---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CustomSecurityAttributeDefinition();


$requestRequestBody->setAttributeSet('Engineering');
$requestRequestBody->setDescription('Active projects for user');
$requestRequestBody->setIsCollection(True);
$requestRequestBody->setIsSearchable(True);
$requestRequestBody->setName('Project');
$requestRequestBody->setStatus('Available');
$requestRequestBody->setType('String');
$requestRequestBody->setUsePreDefinedValuesOnly(True);
$result =  $graphClient->directory()->customSecurityAttributeDefinitions()->post($requestRequestBody);


```