---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UploadClientCertificatePostRequestBody();
requestBody.setPkcs12Value('eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA');

requestBody.setPassword('<password>');



result = await client.identity().apiConnectorsById('identityApiConnector-id').uploadClientCertificate().post(requestBody);


```