---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new InferenceClassificationOverride();


$requestRequestBody->setClassifyAs(new InferenceClassificationType('focused'));
$result =  $graphClient->me()->inferenceClassification()->overridesById('inferenceClassificationOverride-id')->patch($requestRequestBody);


```