---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = O_auth2_permission_grant()
request_body.scope = 'User.Read.All'




result = await client.oauth2_permission_grants.by_oauth2_permission_grant_id('oAuth2PermissionGrant-id').patch(request_body = request_body)


```