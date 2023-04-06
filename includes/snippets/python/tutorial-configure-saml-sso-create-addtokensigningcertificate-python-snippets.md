---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddTokenSigningCertificatePostRequestBody()
request_body.setDisplayName('CN=AWSContoso')

request_body.setEndDateTime(DateTime('2024-01-25T00:00:00Z'))


request_config = AddTokenSigningCertificateRequestBuilderPostRequestConfiguration(
request_config = AddTokenSigningCertificateRequestBuilderPostRequestConfiguration(query_params=)


result = await client.servicePrincipals_by_id('servicePrincipal-id').addTokenSigningCertificate.post(request_body, headers=)


```