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
$allowedValuesArray = [];

$allowedValues1 = new AllowedValue();

$allowedValues1->setId('Alpine');
$allowedValues1->setIsActive(True);

$allowedValuesArray []= $allowedValues1;

$allowedValues2 = new AllowedValue();

$allowedValues2->setId('Baker');
$allowedValues2->setIsActive(True);

$allowedValuesArray []= $allowedValues2;

$allowedValues3 = new AllowedValue();

$allowedValues3->setId('Cascade');
$allowedValues3->setIsActive(True);

$allowedValuesArray []= $allowedValues3;
$requestRequestBody->setAllowedValues($allowedValuesArray);
$result =  $graphClient->directory()->customSecurityAttributeDefinitions()->post($requestRequestBody);


```