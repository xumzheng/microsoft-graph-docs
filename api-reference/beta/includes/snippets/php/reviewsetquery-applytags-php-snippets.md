---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ApplyTagsPostRequestBody();


$tagsToAddArray = [];

$tagsToAddtagsToAdd1 = new Tag();

$tagsToAddtagsToAdd1AdditionalData = [
	"id" => 'b4798d14-748d-468e-a1ec-96a2b1d49677',
];
$tagsToAddtagsToAdd1->setAdditionalData($tagsToAddtagsToAdd1AdditionalData);

$tagsToAddArray []= $tagsToAddtagsToAdd1;
$requestRequestBody->setTagsToAdd($tagsToAddArray);
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->reviewSetsById('reviewSet-id')->queriesById('reviewSetQuery-id')->applyTags()->post($requestRequestBody);


```