---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UploadClientCertificatePostRequestBody
{
	Pkcs12Value = "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
	Password = "<password>",
};
var result = await graphClient.Identity.ApiConnectors["identityApiConnector-id"].UploadClientCertificate.PostAsync(requestBody);


```