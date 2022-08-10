---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new DeviceRegistrationPolicyPostRequestBody
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"id" , "deviceRegistrationPolicy"
		},
		{
			"displayName" , "Device Registration Policy"
		},
		{
			"description" , "Tenant-wide policy that manages intial provisioning controls using quota restrictions, additional authentication and authorization checks"
		},
		{
			"userDeviceQuota" , 50
		},
		{
			"multiFactorAuthConfiguration" , "0"
		},
		{
			"azureADRegistration" , new 
			{
				AppliesTo = "1",
				IsAdminConfigurable = false,
				AllowedUsers = new List<>
				{
				},
				AllowedGroups = new List<>
				{
				},
			}
		},
		{
			"azureADJoin" , new 
			{
				AppliesTo = "1",
				IsAdminConfigurable = true,
				AllowedUsers = new List<>
				{
				},
				AllowedGroups = new List<>
				{
				},
			}
		},
	},
};
await graphClient.DeviceRegistrationPolicy.PutAsync(requestBody);


```