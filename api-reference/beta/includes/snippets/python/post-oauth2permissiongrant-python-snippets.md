---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OAuth2PermissionGrant()
request_body.setClientId('ef969797-201d-4f6b-960c-e9ed5f31dab5')

request_body.setConsentType('AllPrincipals')

request_body.setResourceId('943603e4-e787-4fe9-93d1-e30f749aae39')

request_body.setScope('DelegatedPermissionGrant.ReadWrite.All')

request_body.setStartTime(DateTime('2022-03-17T00:00:00Z'))

request_body.setExpiryTime(DateTime('2023-03-17T00:00:00Z'))



result = await client.oauth2PermissionGrants.post(request_body, headers=)


```