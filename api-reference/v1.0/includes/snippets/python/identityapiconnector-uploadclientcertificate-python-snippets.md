---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UploadClientCertificatePostRequestBody();
$requestBody.setPkcs12Value('eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA');

$requestBody.setPassword('<password>');



$requestResult = $graphServiceClient.identity().apiConnectorsById('identityApiConnector-id').uploadClientCertificate().post($requestBody);


```