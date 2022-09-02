---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AssignLicensePostRequestBody
{
	AddLicenses = new List<AssignedLicense>
	{
		new AssignedLicense
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"disabledPlans" , new List<>
					{
						"8a256a2b-b617-496d-b51b-e76466e88db0",
					}
				},
				{
					"skuId" , "84a661c4-e949-4bd2-a560-ed7766fcaf2b"
				},
			},
		},
		new AssignedLicense
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"disabledPlans" , new List<>
					{
					}
				},
				{
					"skuId" , "f30db892-07e9-47e9-837c-80727f46fd3d"
				},
			},
		},
	},
	RemoveLicenses = new List<>
	{
	},
};
var result = await graphClient.Me.AssignLicense.PostAsync(requestBody);


```