---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CloudPcProvisioningPolicy
{
	OdataType = "#microsoft.graph.cloudPcProvisioningPolicy",
	Description = "Description value",
	DisplayName = "Display Name value",
	DomainJoinConfiguration = new CloudPcDomainJoinConfiguration
	{
		OnPremisesConnectionId = "16ee6c71-fc10-438b-88ac-daa1ccafffff",
		AdditionalData = new Dictionary<string, object>
		{
			{
				"domainJoinType" , "hybridAzureADJoin"
			},
		},
	},
	Id = "1d164206-bf41-4fd2-8424-a3192d39ffff",
	ImageDisplayName = "Windows-10 19h1-evd",
	ImageId = "MicrosoftWindowsDesktop_Windows-10_19h1-evd",
	ImageType = CloudPcProvisioningPolicyImageType.Gallery,
	OnPremisesConnectionId = "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
	WindowsSettings = new CloudPcWindowsSettings
	{
		Language = "en-US",
	},
};
var result = await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies.PostAsync(requestBody);


```