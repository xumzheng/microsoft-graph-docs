---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SelfActivatePostRequestBody()
request_body.setReason('reason-value')

request_body.setDuration('duration-value')

request_body.setTicketNumber('ticketNumber-value')

request_body.setTicketSystem('ticketSystem-value')


request_config = SelfActivateRequestBuilderPostRequestConfiguration(
request_config = SelfActivateRequestBuilderPostRequestConfiguration(query_params=)


result = await client.privilegedRoles_by_id('privilegedRole-id').selfActivate.post(request_body, headers=)


```