---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ApplyTagsPostRequestBody();


$tagsToAddArray = [];

$tagsToAdd1 = new Tag();

$tagsToAdd1AdditionalData = [
		"id" => 'b4798d14-748d-468e-a1ec-96a2b1d49677',
	];
$tagsToAdd1->setAdditionalData($tagsToAdd1AdditionalData);

$tagsToAddArray []= $tagsToAdd1;
$requestRequestBody->setTagsToAdd($tagsToAddArray);
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->reviewSetsById('reviewSet-id')->queriesById('reviewSetQuery-id')->applyTags()->post($requestRequestBody);


```