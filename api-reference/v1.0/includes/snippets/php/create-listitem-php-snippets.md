---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ListItem();



$fields = new FieldValueSet();
$requestRequestBody->setFields($fields);


$fieldsAdditionalData = [
	"Title" => 'Widget',
	"Color" => 'Purple',
	"Weight" => 32,
];
$fields->setAdditionalData($fieldsAdditionalData);

$result =  $graphClient->sitesById('site-id')->listsById('list-id')->items()->post($requestRequestBody);


```