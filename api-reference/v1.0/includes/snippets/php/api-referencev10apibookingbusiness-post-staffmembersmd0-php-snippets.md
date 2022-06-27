---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BookingStaffMemberBase();


$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.bookingStaffMember',
	"displayName" => 'Dana Swope',
	"emailAddress" => 'danas@contoso.com',
	"role@odata.type" => '#microsoft.graph.bookingStaffRole',
	"role" => 'externalGuest',
	"timeZone" => 'America/Chicago',
	"useBusinessHours" => True,
	"workingHours@odata.type" => '#Collection(microsoft.graph.bookingWorkHours)',
	"workingHours" => [],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->solutions()->bookingBusinessesById('bookingBusiness-id')->staffMembers()->post($requestRequestBody);


```