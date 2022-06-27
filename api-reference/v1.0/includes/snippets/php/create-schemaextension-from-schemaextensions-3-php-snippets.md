---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SchemaExtension();


$requestRequestBody->setId('courses');
$requestRequestBody->setDescription('Graph Learn training courses extensions');
$requestRequestBody->setTargetTypes(['Group',]);
$requestRequestBody->setOwner('50897f70-a455-4adf-87bc-4cf17091d5ac');
$propertiesArray = [];

$propertiesproperties1 = new ExtensionSchemaProperty();

$propertiesproperties1AdditionalData = [
"name" => 'courseId',
"type" => 'Integer',
];
$propertiesproperties1->setAdditionalData($propertiesproperties1AdditionalData);

$propertiesArray []= $propertiesproperties1;

$propertiesproperties2 = new ExtensionSchemaProperty();

$propertiesproperties2AdditionalData = [
"name" => 'courseName',
"type" => 'String',
];
$propertiesproperties2->setAdditionalData($propertiesproperties2AdditionalData);

$propertiesArray []= $propertiesproperties2;

$propertiesproperties3 = new ExtensionSchemaProperty();

$propertiesproperties3AdditionalData = [
"name" => 'courseType',
"type" => 'String',
];
$propertiesproperties3->setAdditionalData($propertiesproperties3AdditionalData);

$propertiesArray []= $propertiesproperties3;
$requestRequestBody->setProperties($propertiesArray);
$result =  $graphClient->schemaExtensions()->post($requestRequestBody);


```