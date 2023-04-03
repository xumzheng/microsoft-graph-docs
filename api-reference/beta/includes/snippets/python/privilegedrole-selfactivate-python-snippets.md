---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SelfActivatePostRequestBody();
requestBody.setReason('reason-value');

requestBody.setDuration('duration-value');

requestBody.setTicketNumber('ticketNumber-value');

requestBody.setTicketSystem('ticketSystem-value');



requestResult = graphServiceClient.privilegedRolesById('privilegedRole-id').selfActivate().post(requestBody);


```