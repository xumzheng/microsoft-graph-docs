---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new DeviceRegistrationPolicyRequestBody
{
	AdditionalData = new()
	{
		{"id", "deviceRegistrationPolicy"},
		{"displayName", "Device Registration Policy"},
		{"description", "Tenant-wide policy that manages intial provisioning controls using quota restrictions, additional authentication and authorization checks"},
		{"userDeviceQuota", },
		{"multiFactorAuthConfiguration", "0"},
	}
};
await graphClient.DeviceRegistrationPolicy.PutAsync(requestBody);


```