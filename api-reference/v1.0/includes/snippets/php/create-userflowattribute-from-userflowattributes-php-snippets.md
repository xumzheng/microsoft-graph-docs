---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new IdentityUserFlowAttribute();


$requestRequestBody->setDisplayName('Hobby');
$requestRequestBody->setDescription('Your hobby');
$requestRequestBody->setDataType(new IdentityUserFlowAttributeDataType('string'));
$result =  $graphClient->identity()->userFlowAttributes()->post($requestRequestBody);


```