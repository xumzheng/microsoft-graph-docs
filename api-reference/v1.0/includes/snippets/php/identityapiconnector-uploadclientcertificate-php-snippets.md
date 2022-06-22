---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UploadClientCertificatePostRequestBody();


$requestRequestBody->setPkcs12Value('eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA');
$requestRequestBody->setPassword('<password>');
$result =  $graphClient->identity()->apiConnectorsById('identityApiConnector-id')->uploadClientCertificate()->post($requestRequestBody);


```