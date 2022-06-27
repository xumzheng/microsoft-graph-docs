---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Schema();


$requestRequestBody->setBaseType('microsoft.graph.externalItem');
$propertiesArray = [];

$propertiesproperties1 = new Property();

$propertiesproperties1->setName('ticketTitle');
$propertiesproperties1->setType(new PropertyType('string'));
$propertiesproperties1->setIsSearchable('true');
$propertiesproperties1->setIsRetrievable('true');
$labelsArray = [];
'title',$labelsArray []= $labelslabels1;
$propertiesproperties1->setLabels($labelsArray);

$propertiesArray []= $propertiesproperties1;

$propertiesproperties2 = new Property();

$propertiesproperties2->setName('priority');
$propertiesproperties2->setType(new PropertyType('string'));
$propertiesproperties2->setIsQueryable('true');
$propertiesproperties2->setIsRetrievable('true');
$propertiesproperties2->setIsSearchable('false');

$propertiesArray []= $propertiesproperties2;

$propertiesproperties3 = new Property();

$propertiesproperties3->setName('assignee');
$propertiesproperties3->setType(new PropertyType('string'));
$propertiesproperties3->setIsRetrievable('true');

$propertiesArray []= $propertiesproperties3;
$requestRequestBody->setProperties($propertiesArray);
$result =  $graphClient->external()->connectionsById('externalConnection-id')->schema()->patch($requestRequestBody);


```