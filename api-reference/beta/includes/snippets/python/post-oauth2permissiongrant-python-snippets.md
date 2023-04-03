---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = OAuth2PermissionGrant();
requestBody.setClientId('ef969797-201d-4f6b-960c-e9ed5f31dab5');

requestBody.setConsentType('AllPrincipals');

requestBody.setResourceId('943603e4-e787-4fe9-93d1-e30f749aae39');

requestBody.setScope('DelegatedPermissionGrant.ReadWrite.All');

requestBody.setStartTime(DateTime('2022-03-17T00:00:00Z'));

requestBody.setExpiryTime(DateTime('2023-03-17T00:00:00Z'));



result = await client.oauth2PermissionGrants().post(requestBody);


```