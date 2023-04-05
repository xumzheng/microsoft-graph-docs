---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CrossTenantAccessPolicy()
request_body.setAllowedCloudEndpoints(['microsoftonline.us', 'partner.microsoftonline.cn', ])



result = await client.policies_crossTenantAccessPolicy.patch(request_body)


```