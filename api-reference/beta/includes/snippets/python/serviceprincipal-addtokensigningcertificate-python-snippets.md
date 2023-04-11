---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddTokenSigningCertificatePostRequestBody()
request_body.displayName = 'CN=customDisplayName'

request_body.endDateTime = DateTime('2024-01-25T00:00:00Z')



request_configuration = AddTokenSigningCertificateRequestBuilderPostRequestConfiguration(
)


result = await client.servicePrincipals_by_id('servicePrincipal-id').addTokenSigningCertificate.post(request_body = request_body)


```