---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BookingStaffMemberBase();


$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.bookingStaffMember',
	"workingHours" => [],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->solutions()->bookingBusinessesById('bookingBusiness-id')->staffMembersById('bookingStaffMemberBase-id')->patch($requestRequestBody);


```