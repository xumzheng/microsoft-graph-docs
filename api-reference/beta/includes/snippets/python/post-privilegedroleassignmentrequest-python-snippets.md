---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = PrivilegedRoleAssignmentRequest();
request_body.setDuration('2');

request_body.setReason('Activate the role for business purpose');

request_body.setTicketNumber('234');

request_body.setTicketSystem('system');

schedule = GovernanceSchedule();
schedule.setStartDateTime(DateTime('2018-02-08T02:35:17.903Z'));


request_body.setSchedule($schedule);
request_body.setType('UserAdd');

request_body.setAssignmentState('Active');

request_body.setRoleId('88d8e3e3-8f55-4a1e-953a-9b9898b8876b');



result = await client.privilegedRoleAssignmentRequests().post(request_body);


```