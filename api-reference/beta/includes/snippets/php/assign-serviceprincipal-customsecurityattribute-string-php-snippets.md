---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ServicePrincipal();



$customSecurityAttributes = new CustomSecurityAttributeValue();
$requestRequestBody->setCustomSecurityAttributes($customSecurityAttributes);


$customSecurityAttributesAdditionalData = [
];
$customSecurityAttributes->setAdditionalData($customSecurityAttributesAdditionalData);

$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->patch($requestRequestBody);


```