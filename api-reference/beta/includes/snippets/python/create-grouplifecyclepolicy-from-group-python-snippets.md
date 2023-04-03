---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = GroupLifecyclePolicy();
requestBody.setGroupLifetimeInDays(100);

requestBody.setManagedGroupTypes('Selected');

requestBody.setAlternateNotificationEmails('admin@contoso.com');



result = awaitclient.groupLifecyclePolicies().post(requestBody);


```