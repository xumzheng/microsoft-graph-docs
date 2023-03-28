---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new BookingBusiness();
$requestBody->setEmail('admin@fabrikam.com');

$schedulingPolicy = new BookingSchedulingPolicy();
$schedulingPolicy->setTimeSlotInterval(new \DateInterval('PT60M'));

$schedulingPolicy->setMinimumLeadTime(new \DateInterval('P1D'));

$schedulingPolicy->setMaximumAdvance(new \DateInterval('P30D'));

$schedulingPolicy->setSendConfirmationsToOwner(true);

$schedulingPolicy->setAllowStaffSelection(true);


$requestBody->setSchedulingPolicy($schedulingPolicy);


$requestResult = $graphServiceClient->bookingBusinessesById('bookingBusiness-id')->patch($requestBody);


```