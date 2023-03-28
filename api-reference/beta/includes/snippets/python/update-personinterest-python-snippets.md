---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PersonInterest();
$requestBody->setCategories(['Sports', ]);



$requestResult = $graphServiceClient->me()->profile()->interestsById('personInterest-id')->patch($requestBody);


```