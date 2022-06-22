---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Schema();


$requestRequestBody->setBaseType('microsoft.graph.externalItem');
$propertiesArray = [];

$properties1 = new Property();

$properties1->setName('ticketTitle');
$properties1->setType(new PropertyType('string'));
$properties1->setIsSearchable('true');
$properties1->setIsRetrievable('true');
$labelsArray = [];
'title',$labelsArray []= $labels1;
$properties1->setLabels($labelsArray);

$propertiesArray []= $properties1;

$properties2 = new Property();

$properties2->setName('priority');
$properties2->setType(new PropertyType('string'));
$properties2->setIsQueryable('true');
$properties2->setIsRetrievable('true');
$properties2->setIsSearchable('false');

$propertiesArray []= $properties2;

$properties3 = new Property();

$properties3->setName('assignee');
$properties3->setType(new PropertyType('string'));
$properties3->setIsRetrievable('true');

$propertiesArray []= $properties3;
$requestRequestBody->setProperties($propertiesArray);
$result =  $graphClient->external()->connectionsById('externalConnection-id')->schema()->patch($requestRequestBody);


```