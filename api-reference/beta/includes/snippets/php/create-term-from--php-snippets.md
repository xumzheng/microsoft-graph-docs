---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Term();


$labelsArray = [];

$labels1 = new LocalizedLabel();

$labels1->setLanguageTag('en-US');
$labels1->setName('Car');
$labels1->setIsDefault(True);

$labelsArray []= $labels1;
$requestRequestBody->setLabels($labelsArray);
$result =  $graphClient->termStore()->setsById('set-id')->children()->post($requestRequestBody);


```