---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Term();
$labelsLocalizedLabel1 = new LocalizedLabel();
$labelsLocalizedLabel1->setName('changedLabel');

$labelsLocalizedLabel1->setLanguageTag('en-US');

$labelsLocalizedLabel1->setIsDefault(true);


$labelsArray []= $labelsLocalizedLabel1;
$requestBody->setLabels($labelsArray);




$requestResult = $graphServiceClient->termStore()->setsById('set-id')->termsById('term-id')->patch($requestBody);


```