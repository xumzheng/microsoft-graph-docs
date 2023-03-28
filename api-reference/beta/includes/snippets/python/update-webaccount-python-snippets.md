---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new WebAccount();
$requestBody->setWebUrl('https://github.com/innocenty.popov');



$requestResult = $graphServiceClient->me()->profile()->webAccountsById('webAccount-id')->patch($requestBody);


```