---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CloudPcDeviceImage
{
	OdataType = "#microsoft.graph.cloudPcDeviceImage",
	DisplayName = "Display Name value",
	OsBuildNumber = "OS Build Number value",
	OperatingSystem = "Operating System value",
	Version = "Version value",
	SourceImageResourceId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage",
};
var result = await graphClient.DeviceManagement.VirtualEndpoint.DeviceImages.PostAsync(requestBody);


```