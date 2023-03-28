---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PersonName();
$requestBody->setDisplayName('Innocenty Popov');

$requestBody->setFirst('Innocenty');

$requestBody->setInitials('IP');

$requestBody->setLast('Popov');

$requestBody->setLanguageTag('en-US');

$requestBody->setMaiden(null);



$requestResult = $graphServiceClient->me()->profile()->names()->post($requestBody);


```