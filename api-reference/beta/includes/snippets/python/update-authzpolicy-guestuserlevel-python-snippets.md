---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthorizationPolicy()
additionalData = [
'guestUserRole' => '2af84b1e-32c8-42b7-82bc-daa82404023b', 
];
request_body.additionaldata(additionalData)





result = await client.policies.authorizationPolicy_by_id('authorizationPolicy-id').patch(request_body = request_body)


```