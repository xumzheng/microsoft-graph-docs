---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new RequestIdsRequestBody();


$requestRequestBody->setRequestIds(['f01c6af6-6683-4a37-a945-0a925501eede','42bf60ac-d0cb-4206-aa5c-101884298f55','f09c8f14-8d8e-42cf-8a7e-732b0594e79b',]);
$result =  $graphClient->auditLogs()->signIns()->confirmCompromised()->post($requestRequestBody);


```