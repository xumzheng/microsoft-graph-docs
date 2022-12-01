---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SecureScoreControlProfile
{
	VendorInformation = new SecurityVendorInformation
	{
		Provider = "SecureScore",
		ProviderVersion = null,
		SubProvider = null,
		Vendor = "Microsoft",
	},
	AdditionalData = new Dictionary<string, object>
	{
		{
			"assignedTo" , ""
		},
		{
			"comment" , "control is reviewed"
		},
		{
			"state" , "Reviewed"
		},
	},
};
var result = await graphClient.Security.SecureScoreControlProfiles["secureScoreControlProfile-id"].PatchAsync(requestBody);


```