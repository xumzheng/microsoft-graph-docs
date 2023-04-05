---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UploadClientCertificatePostRequestBody()
request_body.setPkcs12Value('eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA')

request_body.setPassword('<password>')



result = await client.identity.apiConnectorsById('identityApiConnector-id').uploadClientCertificate.post(request_body)


```