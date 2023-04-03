---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = MakePermanentPostRequestBody();
requestBody.setReason('reason-value');

requestBody.setTicketNumber('ticketNumber-value');

requestBody.setTicketSystem('ticketSystem-value');



result = awaitclient.privilegedRoleAssignmentsById('privilegedRoleAssignment-id').makePermanent().post(requestBody);


```