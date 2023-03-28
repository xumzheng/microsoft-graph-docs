---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new OutlookCategory();
$requestBody->setDisplayName('Project expenses');

$requestBody->setColor(new CategoryColor('preset9'));



$requestResult = $graphServiceClient->me()->outlook()->masterCategories()->post($requestBody);


```