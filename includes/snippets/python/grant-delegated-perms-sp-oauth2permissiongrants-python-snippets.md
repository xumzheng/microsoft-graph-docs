---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = OAuth2PermissionGrant();
requestBody.setClientId('b0d9b9e3-0ecf-4bfd-8dab-9273dd055a94');

requestBody.setConsentType('Principal');

requestBody.setResourceId('7ea9e944-71ce-443d-811c-71e8047b557a');

requestBody.setPrincipalId('3fbd929d-8c56-4462-851e-0eb9a7b3a2a5');

requestBody.setScope('User.Read.All Group.Read.All');



result = await client.oauth2PermissionGrants().post(requestBody);


```