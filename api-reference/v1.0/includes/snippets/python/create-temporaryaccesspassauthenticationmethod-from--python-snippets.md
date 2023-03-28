---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new TemporaryAccessPassAuthenticationMethod();
$requestBody->setStartDateTime(new DateTime('2022-06-05T00:00:00.000Z'));

$requestBody->setLifetimeInMinutes(60);

$requestBody->setIsUsableOnce(false);



$requestResult = $graphServiceClient->usersById('user-id')->authentication()->temporaryAccessPassMethods()->post($requestBody);


```