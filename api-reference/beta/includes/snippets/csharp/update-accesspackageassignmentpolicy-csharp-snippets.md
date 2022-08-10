---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessPackageAssignmentPolicie
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"id" , "b2eba9a1-b357-42ee-83a8-336522ed6cbf"
		},
		{
			"accessPackageId" , "4c02f928-7752-49aa-8fc8-e286d973a965"
		},
		{
			"displayName" , "All Users"
		},
		{
			"description" , "All users can request for access to the directory."
		},
		{
			"canExtend" , false
		},
		{
			"durationInDays" , 365
		},
		{
			"expirationDateTime" , null
		},
		{
			"requestorSettings" , new 
			{
				ScopeType = "AllExistingConnectedOrganizationSubjects",
				AcceptRequests = true,
				AllowedRequestors = new List<>
				{
				},
			}
		},
		{
			"requestApprovalSettings" , new 
			{
				IsApprovalRequired = true,
				IsApprovalRequiredForExtension = false,
				IsRequestorJustificationRequired = true,
				ApprovalMode = "SingleStage",
				ApprovalStages = new List<>
				{
					new 
					{
						ApprovalStageTimeOutInDays = 14,
						IsApproverJustificationRequired = true,
						IsEscalationEnabled = false,
						EscalationTimeInMinutes = 11520,
						PrimaryApprovers = new List<>
						{
							new 
							{
								OdataType = "#microsoft.graph.groupMembers",
								IsBackup = true,
								Id = "d2dcb9a1-a445-42ee-83a8-476522ed6cbf",
								Description = "group for users from connected organizations which have no external sponsor",
							},
							new 
							{
								OdataType = "#microsoft.graph.externalSponsors",
								IsBackup = false,
							},
						},
					},
				},
			}
		},
		{
			"questions" , new List<>
			{
				new 
				{
					IsRequired = false,
					Text = new 
					{
						DefaultText = "what state are you from?",
						LocalizedTexts = new List<>
						{
							new 
							{
								Text = "¿De qué estado eres?",
								LanguageCode = "es",
							},
						},
					},
					OdataType = "#microsoft.graph.accessPackageMultipleChoiceQuestion",
					Choices = new List<>
					{
						new 
						{
							ActualValue = "AZ",
							DisplayValue = new 
							{
								LocalizedTexts = new List<>
								{
									new 
									{
										Text = "Arizona",
										LanguageCode = "es",
									},
								},
							},
						},
						new 
						{
							ActualValue = "CA",
							DisplayValue = new 
							{
								LocalizedTexts = new List<>
								{
									new 
									{
										Text = "California",
										LanguageCode = "es",
									},
								},
							},
						},
					},
					AllowsMultipleSelection = false,
				},
				new 
				{
					IsRequired = false,
					Text = new 
					{
						DefaultText = "Who is your manager?",
						LocalizedTexts = new List<>
						{
							new 
							{
								Text = "por qué necesita acceso a este paquete",
								LanguageCode = "es",
							},
						},
					},
					OdataType = "#microsoft.graph.accessPackageTextInputQuestion",
					IsSingleLineQuestion = false,
				},
			}
		},
	},
};
await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentPolicies["accessPackageAssignmentPolicy-id"].PutAsync(requestBody);


```