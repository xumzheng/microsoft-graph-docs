---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingBusiness()
request_body.email = 'admin@fabrikam.com'

schedulingPolicy = BookingSchedulingPolicy()
schedulingPolicy.timeslotinterval =  \DateInterval('PT60M')

schedulingPolicy.minimumleadtime =  \DateInterval('P1D')

schedulingPolicy.maximumadvance =  \DateInterval('P30D')

schedulingPolicy.sendConfirmationsToOwner = true

schedulingPolicy.allowStaffSelection = true


request_body.schedulingPolicy = schedulingPolicy


request_configuration = BookingBusinessRequestBuilderPatchRequestConfiguration(
)


result = await client.solutions.bookingBusinesses_by_id('bookingBusiness-id').patch(request_body = request_body)


```