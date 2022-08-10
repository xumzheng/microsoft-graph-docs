---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CloudPcOrganizationSettings
{
	OdataType = "#microsoft.graph.cloudPcOrganizationSettings",
	UserAccountType = CloudPcUserAccountType.Standarduser,
	OsVersion = CloudPcOperatingSystem.Windows11,
	WindowsSettings = new CloudPcWindowsSettings
	{
		Language = "en-US",
	},
};
await graphClient.DeviceManagement.VirtualEndpoint.OrganizationSettings.PatchAsync(requestBody);


```