---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ColumnDefinition();


$requestRequestBody->setRequired(True);
$requestRequestBody->setHidden(False);
$requestRequestBody->setPropagateChanges(False);
$result =  $graphClient->sitesById('site-id')->contentTypesById('contentType-id')->columnsById('columnDefinition-id')->patch($requestRequestBody);


```