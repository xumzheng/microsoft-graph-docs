---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Device
{
	AccountEnabled = true,
	AlternativeSecurityIds = new List<AlternativeSecurityId>
	{
		new AlternativeSecurityId
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"type" , 99
				},
				{
					"identityProvider" , "identityProvider-value"
				},
				{
					"key" , "base64Y3YxN2E1MWFlYw=="
				},
			},
		},
	},
	ApproximateLastSignInDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
	DeviceId = "deviceId-value",
	DeviceMetadata = "deviceMetadata-value",
	DeviceVersion = 99,
};
var result = await graphClient.Devices.PostAsync(requestBody);


```