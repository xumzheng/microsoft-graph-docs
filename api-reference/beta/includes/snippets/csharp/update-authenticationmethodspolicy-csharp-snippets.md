---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AuthenticationMethodsPolicy
{
	RegistrationEnforcement = new RegistrationEnforcement
	{
		AuthenticationMethodsRegistrationCampaign = new AuthenticationMethodsRegistrationCampaign
		{
			SnoozeDurationInDays = 1,
			State = "enabled",
			ExcludeTargets = new List<ExcludeTarget>
			{
			}
			IncludeTargets = new List<AuthenticationMethodsRegistrationCampaignIncludeTarget>
			{
				new AuthenticationMethodsRegistrationCampaignIncludeTarget
				{
					AdditionalData = new()
					{
						{"id", "3ee3a9de-0a86-4e12-a287-9769accf1ba2"},
						{"targetType", "group"},
						{"targetedAuthenticationMethod", "microsoftAuthenticator"},
					}
				},
			}
		},
	},
};
await graphClient.Policies.AuthenticationMethodsPolicy.PatchAsync(requestBody);


```