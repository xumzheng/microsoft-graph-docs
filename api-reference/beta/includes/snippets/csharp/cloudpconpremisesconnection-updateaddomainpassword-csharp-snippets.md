---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.DeviceManagement.VirtualEndpoint.OnPremisesConnections.Item.MicrosoftGraphUpdateAdDomainPassword.UpdateAdDomainPasswordPostRequestBody
{
	AdDomainPassword = "AdDomainPassword value",
};
await graphClient.DeviceManagement.VirtualEndpoint.OnPremisesConnections["cloudPcOnPremisesConnection-id"].MicrosoftGraphUpdateAdDomainPassword.PostAsync(requestBody);


```