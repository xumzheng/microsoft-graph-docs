---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.ServicePrincipals.Item.AddTokenSigningCertificate.AddTokenSigningCertificatePostRequestBody
{
	DisplayName = "CN=customDisplayName",
	EndDateTime = DateTimeOffset.Parse("2024-01-25T00:00:00Z"),
};
var result = await graphClient.ServicePrincipals["servicePrincipal-id"].AddTokenSigningCertificate.PostAsync(requestBody);


```