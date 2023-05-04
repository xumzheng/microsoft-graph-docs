---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Authentication_flows_policy()
self_service_sign_up = Self_service_sign_up_authentication_flow_configuration()
self_service_sign_up.is_enabled = True


request_body.self_service_sign_up = self_service_sign_up



result = await client.policies.authentication_flow_policy.patch(request_body = request_body)


```