---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = GroupLifecyclePolicy();
requestBody.setGroupLifetimeInDays(180);

requestBody.setManagedGroupTypes('Selected');

requestBody.setAlternateNotificationEmails('admin@contoso.com');



result = awaitclient.groupLifecyclePoliciesById('groupLifecyclePolicy-id').patch(requestBody);


```