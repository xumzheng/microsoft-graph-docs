---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = BookingBusiness()
request_body.setEmail('admin@fabrikam.com')

schedulingPolicy = BookingSchedulingPolicy()
$schedulingPolicy.setTimeSlotInterval( \DateInterval('PT60M'))

$schedulingPolicy.setMinimumLeadTime( \DateInterval('P1D'))

$schedulingPolicy.setMaximumAdvance( \DateInterval('P30D'))

schedulingPolicy.setSendConfirmationsToOwner(true)

schedulingPolicy.setAllowStaffSelection(true)


request_body.setSchedulingPolicy($schedulingPolicy)


result = await client.solutions.bookingBusinessesById('bookingBusiness-id').patch(request_body)


```