---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new IdentityUserFlowAttribute();


$requestRequestBody->setDescription('Your new hobby');
$result =  $graphClient->identity()->userFlowAttributesById('identityUserFlowAttribute-id')->patch($requestRequestBody);


```