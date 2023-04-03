---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PrivilegedRoleAssignmentRequest();
requestBody.setDuration('2');

requestBody.setReason('Activate the role for business purpose');

requestBody.setTicketNumber('234');

requestBody.setTicketSystem('system');

schedule = GovernanceSchedule();
schedule.setStartDateTime(DateTime('2018-02-08T02:35:17.903Z'));


requestBody.setSchedule($schedule);
requestBody.setType('UserAdd');

requestBody.setAssignmentState('Active');

requestBody.setRoleId('88d8e3e3-8f55-4a1e-953a-9b9898b8876b');



result = await client.privilegedRoleAssignmentRequests().post(requestBody);


```