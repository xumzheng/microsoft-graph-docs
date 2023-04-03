---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = TimeOffReason();
requestBody.setDisplayName('Vacation');

requestBody.setIconType(TimeOffReasonIconType('plane'));

requestBody.setIsActive(true);



requestResult = graphServiceClient.teamsById('team-id').schedule().timeOffReasons().post(requestBody);


```