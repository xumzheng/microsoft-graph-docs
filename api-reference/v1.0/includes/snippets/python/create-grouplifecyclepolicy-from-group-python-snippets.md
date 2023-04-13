---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GroupLifecyclePolicy()
request_body.group_lifetime_in_days = 100

request_body.managedGroupTypes = 'Selected'

request_body.alternateNotificationEmails = 'admin@contoso.com'




result = await client.groupLifecyclePolicies.post(request_body = request_body)


```