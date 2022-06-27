---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ServicePrincipal();


$requestRequestBody->setAppId('65415bb1-9267-4313-bbf5-ae259732ee12');
$result =  $graphClient->servicePrincipals()->post($requestRequestBody);


```