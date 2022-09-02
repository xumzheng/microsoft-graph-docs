---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CreatePostRequestBody
{
	DisplayName = "Test Printer",
	Manufacturer = "Test Printer Manufacturer",
	Model = "Test Printer Model",
	PhysicalDeviceId = null,
	HasPhysicalDevice = false,
	CertificateSigningRequest = new PrintCertificateSigningRequest
	{
		Content = "{content}",
		TransportKey = "{sampleTransportKey}",
	},
	ConnectorId = null,
};
await graphClient.Print.Printers.Create.PostAsync(requestBody);


```