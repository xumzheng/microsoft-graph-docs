---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ActivityBasedTimeoutPolicy()
request_body.setDefinition(['definition-value', ])

request_body.setDisplayName('displayName-value')

request_body.setIsOrganizationDefault(true)


request_config = ActivityBasedTimeoutPoliciesRequestBuilderPostRequestConfiguration(
request_config = ActivityBasedTimeoutPoliciesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.policies.activityBasedTimeoutPolicies.post(request_body, headers=)


```