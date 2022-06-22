---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BookingBusiness();


$requestRequestBody->setEmail('admin@fabrikam.com');

$schedulingPolicy = new BookingSchedulingPolicy();
$requestRequestBody->setSchedulingPolicy($schedulingPolicy);


$schedulingPolicy->setTimeSlotInterval('PT60M');
$schedulingPolicy->setMinimumLeadTime('P1D');
$schedulingPolicy->setMaximumAdvance('P30D');
$schedulingPolicy->setSendConfirmationsToOwner(True);
$schedulingPolicy->setAllowStaffSelection(True);

$result =  $graphClient->bookingBusinessesById('bookingBusiness-id')->patch($requestRequestBody);


```