---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingBusiness()
request_body.email = 'admin@fabrikam.com'

scheduling_policy = BookingSchedulingPolicy()
schedulingPolicy.timeslotinterval =  \DateInterval('PT60M')

schedulingPolicy.minimumleadtime =  \DateInterval('P1D')

schedulingPolicy.maximumadvance =  \DateInterval('P30D')

schedulingPolicy.send_confirmations_to_owner = True

schedulingPolicy.allow_staff_selection = True


request_body.scheduling_policy = schedulingPolicy



result = await client.bookingBusinesses_by_id('bookingBusiness-id').patch(request_body = request_body)


```