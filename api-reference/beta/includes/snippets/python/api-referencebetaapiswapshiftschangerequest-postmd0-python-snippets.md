---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SwapShiftsChangeRequest()
request_body.setSenderShiftId('5ad10161-6524-4c7c-9beb-4e8677ba2f6d')

request_body.setSenderMessage('I can\'t make my shift, any chance we can swap?')

request_body.setRecipientUserId('567c8ea5-9e32-422a-a663-8270201699cd')

request_body.setRecipientShiftId('e73408ca-3ea5-4bbf-96a8-2e06c95f7a2c')


request_configuration = SwapShiftsChangeRequestsRequestBuilderPostRequestConfiguration(
request_configuration = SwapShiftsChangeRequestsRequestBuilderPostRequestConfiguration(query_params=)
System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.teams_by_id('team-id').schedule.swapShiftsChangeRequests.post(request_body, request_configuration)


```