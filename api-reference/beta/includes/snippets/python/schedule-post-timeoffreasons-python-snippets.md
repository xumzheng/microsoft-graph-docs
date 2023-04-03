---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = TimeOffReason();
requestBody.setDisplayName('Vacation');

requestBody.setIconType(TimeOffReasonIconType('plane'));

requestBody.setIsActive(true);



result = await client.teamsById('team-id').schedule().timeOffReasons().post(requestBody);


```