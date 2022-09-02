---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ReprovisionPostRequestBody
{
	UserAccountType = CloudPcUserAccountType.Administrator,
	OsVersion = CloudPcOperatingSystem.Windows10,
};
await graphClient.DeviceManagement.VirtualEndpoint.CloudPCs["cloudPC-id"].Reprovision.PostAsync(requestBody);


```