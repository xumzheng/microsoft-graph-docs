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

$allowedValuesallowedValues1 = new AllowedValue();

$allowedValuesallowedValues1->setId('Alpine');
$allowedValuesallowedValues1->setIsActive(True);

$allowedValuesArray []= $allowedValuesallowedValues1;

$allowedValuesallowedValues2 = new AllowedValue();

$allowedValuesallowedValues2->setId('Baker');
$allowedValuesallowedValues2->setIsActive(True);

$allowedValuesArray []= $allowedValuesallowedValues2;

$allowedValuesallowedValues3 = new AllowedValue();

$allowedValuesallowedValues3->setId('Cascade');
$allowedValuesallowedValues3->setIsActive(True);

$allowedValuesArray []= $allowedValuesallowedValues3;
$requestRequestBody->setAllowedValues($allowedValuesArray);
$result =  $graphClient->directory()->customSecurityAttributeDefinitions()->post($requestRequestBody);


```