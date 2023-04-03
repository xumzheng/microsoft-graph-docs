---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = GroupLifecyclePolicy();
requestBody.setGroupLifetimeInDays(180);

requestBody.setManagedGroupTypes('Selected');

requestBody.setAlternateNotificationEmails('admin@contoso.com');



result = await client.groupLifecyclePoliciesById('groupLifecyclePolicy-id').patch(requestBody);


```