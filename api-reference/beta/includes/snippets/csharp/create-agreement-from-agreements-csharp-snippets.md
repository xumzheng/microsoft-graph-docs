---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Agreement
{
	DisplayName = "Contoso ToU for guest users",
	IsViewingBeforeAcceptanceRequired = true,
	Files = new List<AgreementFileLocalization>
	{
		new AgreementFileLocalization
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"fileName" , "TOU.pdf"
				},
				{
					"language" , "en"
				},
				{
					"isDefault" , true
				},
				{
					"fileData" , new 
					{
						Data = "SGVsbG8gd29ybGQ=//truncated-binary",
					}
				},
			},
		},
	},
};
var result = await graphClient.IdentityGovernance.TermsOfUse.Agreements.PostAsync(requestBody);


```