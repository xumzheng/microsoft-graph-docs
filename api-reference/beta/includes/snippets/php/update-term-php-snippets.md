---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Term();


$labelsArray = [];

$labelslabels1 = new LocalizedLabel();

$labelslabels1->setName('changedLabel');
$labelslabels1->setLanguageTag('en-US');
$labelslabels1->setIsDefault(True);

$labelsArray []= $labelslabels1;
$requestRequestBody->setLabels($labelsArray);
$result =  $graphClient->termStore()->setsById('set-id')->termsById('term-id')->patch($requestRequestBody);


```