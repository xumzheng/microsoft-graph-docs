---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SecureScoreControlProfile();



$vendorInformation = new SecurityVendorInformation();
$requestRequestBody->setVendorInformation($vendorInformation);


$vendorInformation->setProvider('SecureScore');
$vendorInformation->setProviderVersion(null);
$vendorInformation->setSubProvider(null);
$vendorInformation->setVendor('Microsoft');

$requestRequestBodyAdditionalData = [
"assignedTo" => '',
"comment" => 'control is reviewed',
"state" => 'Reviewed',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->security()->secureScoreControlProfilesById('secureScoreControlProfile-id')->patch($requestRequestBody);


```