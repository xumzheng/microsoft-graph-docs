---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = GroupLifecyclePolicy();
request_body.setGroupLifetimeInDays(100);

request_body.setManagedGroupTypes('Selected');

request_body.setAlternateNotificationEmails('admin@contoso.com');



result = await client.groupLifecyclePolicies().post(request_body);


```