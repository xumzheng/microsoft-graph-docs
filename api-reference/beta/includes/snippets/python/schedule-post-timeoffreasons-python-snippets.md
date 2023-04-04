---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = TimeOffReason();
request_body.setDisplayName('Vacation');

request_body.setIconType(TimeOffReasonIconType('plane'));

request_body.setIsActive(true);



result = await client.teamsById('team-id').schedule().timeOffReasons().post(request_body);


```