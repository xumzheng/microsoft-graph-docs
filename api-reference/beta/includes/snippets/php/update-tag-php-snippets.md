---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Tag();


$requestRequestBody->setDescription('This is an updated description.');
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->tagsById('tag-id')->patch($requestRequestBody);


```