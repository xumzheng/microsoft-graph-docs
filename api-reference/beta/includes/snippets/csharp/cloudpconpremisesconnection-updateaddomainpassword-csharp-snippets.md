---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.DeviceManagement.VirtualEndpoint.OnPremisesConnections.Item.UpdateAdDomainPassword.UpdateAdDomainPasswordPostRequestBody
{
	AdDomainPassword = "AdDomainPassword value",
};
await graphClient.DeviceManagement.VirtualEndpoint.OnPremisesConnections["cloudPcOnPremisesConnection-id"].UpdateAdDomainPassword.PostAsync(requestBody);


```