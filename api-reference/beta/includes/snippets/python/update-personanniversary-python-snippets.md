---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PersonAnnualEvent();
$requestBody->setAllowedAudiences(new AllowedAudiences('contacts'));



$requestResult = $graphServiceClient->me()->profile()->anniversariesById('personAnnualEvent-id')->patch($requestBody);


```