---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MakePermanentPostRequestBody()
request_body.setReason('reason-value')

request_body.setTicketNumber('ticketNumber-value')

request_body.setTicketSystem('ticketSystem-value')


request_config = MakePermanentRequestBuilderPostRequestConfiguration(
request_config = MakePermanentRequestBuilderPostRequestConfiguration(query_params=)


result = await client.privilegedRoleAssignments_by_id('privilegedRoleAssignment-id').makePermanent.post(request_body, headers=)


```