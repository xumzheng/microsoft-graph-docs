---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CloudPcOrganizationSettings
{
	@odata.type = "#microsoft.graph.cloudPcOrganizationSettings",
	UserAccountType = "standardUser",
	OsVersion = "windows11",
	WindowsSettings = new CloudPcWindowsSettings
	{
		Language = "en-US",
	},
};
await graphClient.DeviceManagement.VirtualEndpoint.OrganizationSettings.PatchAsync(requestBody);


```