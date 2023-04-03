---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = BookingBusiness();
requestBody.setEmail('admin@fabrikam.com');

schedulingPolicy = BookingSchedulingPolicy();
$schedulingPolicy.setTimeSlotInterval( \DateInterval('PT60M'));

$schedulingPolicy.setMinimumLeadTime( \DateInterval('P1D'));

$schedulingPolicy.setMaximumAdvance( \DateInterval('P30D'));

schedulingPolicy.setSendConfirmationsToOwner(true);

schedulingPolicy.setAllowStaffSelection(true);


requestBody.setSchedulingPolicy($schedulingPolicy);


requestResult = graphServiceClient.solutions().bookingBusinessesById('bookingBusiness-id').patch(requestBody);


```