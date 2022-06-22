---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SchemaExtension();


$requestRequestBody->setId('graphlearn_courses');
$requestRequestBody->setDescription('Graph Learn training courses extensions');
$requestRequestBody->setTargetTypes( [
'Group',],
$propertiesArray = [];

$properties1 = new ExtensionSchemaProperty();

$properties1AdditionalData = [
		"name" => 'courseId',
		"type" => 'Integer',
	];
$properties1->setAdditionalData($properties1AdditionalData);

$propertiesArray []= $properties1;

$properties2 = new ExtensionSchemaProperty();

$properties2AdditionalData = [
	"name" => 'courseName',
	"type" => 'String',
];
$properties2->setAdditionalData($properties2AdditionalData);

$propertiesArray []= $properties2;

$properties3 = new ExtensionSchemaProperty();

$properties3AdditionalData = [
"name" => 'courseType',
"type" => 'String',
];
$properties3->setAdditionalData($properties3AdditionalData);

$propertiesArray []= $properties3;
$requestRequestBody->setProperties($propertiesArray);
$result =  $graphClient->schemaExtensions()->post($requestRequestBody);


```