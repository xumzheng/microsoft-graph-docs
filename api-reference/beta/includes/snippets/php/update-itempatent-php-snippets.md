---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ItemPatent();


$requestRequestBody->setNumber('USPTO-3954432633');
$requestRequestBody->setWebUrl('https://patents.gov/3954432633');
$result =  $graphClient->usersById('user-id')->profile()->patentsById('itemPatent-id')->patch($requestRequestBody);


```