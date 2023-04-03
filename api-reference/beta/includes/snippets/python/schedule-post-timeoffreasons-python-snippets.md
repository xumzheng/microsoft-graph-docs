---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = TimeOffReason();
requestBody.setDisplayName('Vacation');

requestBody.setIconType(TimeOffReasonIconType('plane'));

requestBody.setIsActive(true);



result = awaitclient.teamsById('team-id').schedule().timeOffReasons().post(requestBody);


```