---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SelfActivatePostRequestBody();
requestBody.setReason('reason-value');

requestBody.setDuration('duration-value');

requestBody.setTicketNumber('ticketNumber-value');

requestBody.setTicketSystem('ticketSystem-value');



result = await client.privilegedRolesById('privilegedRole-id').selfActivate().post(requestBody);


```