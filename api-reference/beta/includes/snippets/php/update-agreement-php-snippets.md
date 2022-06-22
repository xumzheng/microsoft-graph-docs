---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Agreement();


$requestRequestBody->setDisplayName('All Contoso volunteers - Terms of use');
$requestRequestBody->setIsViewingBeforeAcceptanceRequired(True);
$result =  $graphClient->identityGovernance()->termsOfUse()->agreementsById('agreement-id')->patch($requestRequestBody);


```