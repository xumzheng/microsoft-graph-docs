---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ItemAddress();
requestBody.setAllowedAudiences(AllowedAudiences('me'));

requestBody.setDisplayName('Secret Hideout');



requestResult = graphServiceClient.usersById('user-id').profile().addressesById('itemAddress-id').patch(requestBody);


```