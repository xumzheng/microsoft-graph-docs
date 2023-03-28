---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new MakePermanentPostRequestBody();
$requestBody->setReason('reason-value');

$requestBody->setTicketNumber('ticketNumber-value');

$requestBody->setTicketSystem('ticketSystem-value');



$requestResult = $graphServiceClient->privilegedRoleAssignmentsById('privilegedRoleAssignment-id')->makePermanent()->post($requestBody);


```