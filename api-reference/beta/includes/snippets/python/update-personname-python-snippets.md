---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PersonName();
$requestBody->setNickname('Kesha');



$requestResult = $graphServiceClient->me()->profile()->namesById('personName-id')->patch($requestBody);


```