---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CrossTenantAccessPolicy();


$requestRequestBody->setAllowedCloudEndpoints(['microsoftonline.us','partner.microsoftonline.cn',]);
$result =  $graphClient->policies()->crossTenantAccessPolicy()->patch($requestRequestBody);


```