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
			State = AdvancedConfigState.Enabled,
			ExcludeTargets = new List<>
			{
			},
			IncludeTargets = new List<AuthenticationMethodsRegistrationCampaignIncludeTarget>
			{
				new AuthenticationMethodsRegistrationCampaignIncludeTarget
				{
					AdditionalData = new Dictionary<string, object>
					{
						{
							"id" , "3ee3a9de-0a86-4e12-a287-9769accf1ba2"
						},
						{
							"targetType" , "group"
						},
						{
							"targetedAuthenticationMethod" , "microsoftAuthenticator"
						},
					},
				},
			},
		},
	},
};
await graphClient.Policies.AuthenticationMethodsPolicy.PatchAsync(requestBody);


```