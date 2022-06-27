---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ColumnDefinition();


$requestRequestBodyAdditionalData = [
	"sourceColumn@odata.bind" => 'https://graph.microsoft.com/v1.0/sites/root/columns/99ddcf45-e2f7-4f17-82b0-6fba34445103',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->sitesById('site-id')->contentTypesById('contentType-id')->columns()->post($requestRequestBody);


```