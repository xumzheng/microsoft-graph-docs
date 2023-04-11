---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UploadClientCertificatePostRequestBody()
request_body.pkcs12Value = 'eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA'

request_body.password = '<password>'



request_configuration = UploadClientCertificateRequestBuilderPostRequestConfiguration(
)


result = await client.identity.apiConnectors_by_id('identityApiConnector-id').uploadClientCertificate.post(request_body = request_body)


```