---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ValidatePropertiesPostRequestBody();


$requestRequestBody->setEntityType('Group');
$requestRequestBody->setDisplayName('Myprefix_test_mysuffix');
$requestRequestBody->setMailNickname('Myprefix_test_mysuffix');
$requestRequestBody->setOnBehalfOfUserId('onBehalfOfUserId-value');
$result =  $graphClient->directoryObjects()->validateProperties()->post($requestRequestBody);


```