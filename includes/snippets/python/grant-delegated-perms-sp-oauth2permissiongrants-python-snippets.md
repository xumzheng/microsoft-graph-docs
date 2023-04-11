---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OAuth2PermissionGrant()
request_body.clientId = 'b0d9b9e3-0ecf-4bfd-8dab-9273dd055a94'

request_body.consentType = 'Principal'

request_body.resourceId = '7ea9e944-71ce-443d-811c-71e8047b557a'

request_body.principalId = '3fbd929d-8c56-4462-851e-0eb9a7b3a2a5'

request_body.scope = 'User.Read.All Group.Read.All'



request_configuration = Oauth2PermissionGrantsRequestBuilderPostRequestConfiguration(
)


result = await client.oauth2PermissionGrants.post(request_body = request_body)


```