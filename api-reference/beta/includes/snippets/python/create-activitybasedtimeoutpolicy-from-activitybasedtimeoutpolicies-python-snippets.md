---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ActivityBasedTimeoutPolicy()
request_body.Definition(['definition-value', ])

request_body.displayName = 'displayName-value'

request_body.is_organization_default = True




result = await client.policies.activityBasedTimeoutPolicies.post(request_body = request_body)


```