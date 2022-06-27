---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AdministrativeUnit();


$requestRequestBodyAdditionalData = [
	"membershipType" => 'Dynamic',
	"membershipRule" => '(user.country -eq "United States")',
	"membershipRuleProcessingState" => 'On',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->administrativeUnitsById('administrativeUnit-id')->patch($requestRequestBody);


```