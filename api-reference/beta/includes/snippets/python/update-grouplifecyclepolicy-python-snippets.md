---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GroupLifecyclePolicy()
request_body.groupLifetimeInDays = 180

request_body.managedGroupTypes = 'Selected'

request_body.alternateNotificationEmails = 'admin@contoso.com'




result = await client.groupLifecyclePolicies_by_id('groupLifecyclePolicy-id').patch(request_body = request_body)


```