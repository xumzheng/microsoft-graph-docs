---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ItemPhone();


$requestRequestBody->setType(new PhoneType('other'));
$result =  $graphClient->usersById('user-id')->profile()->phonesById('itemPhone-id')->patch($requestRequestBody);


```