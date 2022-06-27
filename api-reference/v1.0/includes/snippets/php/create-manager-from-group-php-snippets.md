---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ReferenceUpdateSchema();


$requestRequestBody->set@odata.id('https://graph.microsoft.com/v1.0/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0');
$result =  $graphClient->usersById('user-id')->manager()->ref()->put($requestRequestBody);


```