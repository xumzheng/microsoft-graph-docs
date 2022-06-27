---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Ref();


$requestRequestBodyAdditionalData = [
	"@odata.id" => 'https://graph.microsoft.com/odata/groups(\'1a9db3ab-0acf-4808-99ae-e8ed581cb2e0\')',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->policies()->mobileAppManagementPoliciesById('mobilityManagementPolicy-id')->includedGroups()->ref()->post($requestRequestBody);


```