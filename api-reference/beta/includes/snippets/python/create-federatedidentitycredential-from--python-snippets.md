---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = FederatedIdentityCredential()
request_body.setName('testing02')

request_body.setIssuer('https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0')

request_body.setSubject('a7d388c3-5e3f-4959-ac7d-786b3383006a')

request_body.setAudiences(['api://AzureADTokenExchange', ])



result = await client.applications._by_id('application-id').federatedIdentityCredentials.post(request_body)


```