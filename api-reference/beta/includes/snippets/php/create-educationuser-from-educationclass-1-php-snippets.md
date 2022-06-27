---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Ref();


$requestRequestBodyAdditionalData = [
	"@odata.id" => 'https://graph.microsoft.com/beta/education/users/13015',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->education()->classesById('educationClass-id')->members()->ref()->post($requestRequestBody);


```