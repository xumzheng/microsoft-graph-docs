---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UserAccountTypeRequestBody();


$requestRequestBody->setUserAccountType(new CloudPcUserAccountType('administrator'));
$result =  $graphClient->deviceManagement()->virtualEndpoint()->cloudPCsById('cloudPC-id')->changeUserAccountType()->post($requestRequestBody);


```