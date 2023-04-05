---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OAuth2PermissionGrant()
request_body.setScope('User.Read.All')



result = await client.oauth2PermissionGrants._by_id('oAuth2PermissionGrant-id').patch(request_body)


```