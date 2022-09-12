---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CloudPcExternalPartnerSetting
{
	OdataType = "#microsoft.graph.cloudPcExternalPartnerSetting",
	EnableConnection = true,
};
await graphClient.DeviceManagement.VirtualEndpoint.ExternalPartnerSettings["cloudPcExternalPartnerSetting-id"].PatchAsync(requestBody);


```