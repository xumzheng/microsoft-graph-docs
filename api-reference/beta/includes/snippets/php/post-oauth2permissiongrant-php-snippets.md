---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OAuth2PermissionGrant();


$requestRequestBody->setClientId('ef969797-201d-4f6b-960c-e9ed5f31dab5');
$requestRequestBody->setConsentType('AllPrincipals');
$requestRequestBody->setResourceId('943603e4-e787-4fe9-93d1-e30f749aae39');
$requestRequestBody->setScope('DelegatedPermissionGrant.ReadWrite.All');
$requestRequestBody->setStartTime(new DateTime("2022-03-17T00:00:00Z"));
$requestRequestBody->setExpiryTime(new DateTime("2023-03-17T00:00:00Z"));
$result =  $graphClient->oauth2PermissionGrants()->post($requestRequestBody);


```