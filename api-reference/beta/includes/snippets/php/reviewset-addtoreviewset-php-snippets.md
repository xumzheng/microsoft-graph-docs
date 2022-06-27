---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AddToReviewSetPostRequestBody();



$sourceCollection = new SourceCollection();
$requestRequestBody->setSourceCollection($sourceCollection);


$sourceCollection->setId('1a9b4145d8f84e39bc45a7f68c5c5119');

$requestRequestBodyAdditionalData = [
"additionalData" => 'linkedFiles',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->reviewSetsById('reviewSet-id')->addToReviewSet()->post($requestRequestBody);


```