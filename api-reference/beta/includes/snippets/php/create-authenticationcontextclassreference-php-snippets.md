---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AuthenticationContextClassReference();


$requestRequestBody->setId('c1');
$requestRequestBody->setDisplayName('Contoso medium');
$requestRequestBody->setDescription('Medium protection level defined for Contoso policy');
$requestRequestBody->setIsAvailable(True);
$result =  $graphClient->identity()->conditionalAccess()->authenticationContextClassReferences()->post($requestRequestBody);


```