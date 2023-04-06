---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PermissionGrantConditionSet()
request_body.setPermissionType(PermissionType('delegated'))

request_body.setCertifiedClientApplicationsOnly(true)


request_config = IncludesRequestBuilderPostRequestConfiguration(
request_config = IncludesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.policies.permissionGrantPolicies_by_id('permissionGrantPolicy-id').includes.post(request_body, headers=)


```