---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OAuth2PermissionGrant()
request_body.setScope('User.ReadBasic.All Group.ReadWrite.All')


request_config = OAuth2PermissionGrantRequestBuilderPatchRequestConfiguration(
request_config = OAuth2PermissionGrantRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.oauth2PermissionGrants_by_id('oAuth2PermissionGrant-id').patch(request_body, headers=)


```