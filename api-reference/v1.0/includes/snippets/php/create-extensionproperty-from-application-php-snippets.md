---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ExtensionProperty();


$requestRequestBody->setName('jobGroup');
$requestRequestBody->setDataType('String');
$requestRequestBody->setTargetObjects( [
'User',],
$result =  $graphClient->applicationsById('application-id')->extensionProperties()->post($requestRequestBody);


```