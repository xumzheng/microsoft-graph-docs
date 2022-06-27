---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ReprovisionPostRequestBody();


$requestRequestBody->setUserAccountType(new CloudPcUserAccountType('administrator'));
$requestRequestBody->setOsVersion(new CloudPcOperatingSystem('windows10'));
$result =  $graphClient->deviceManagement()->virtualEndpoint()->cloudPCsById('cloudPC-id')->reprovision()->post($requestRequestBody);


```