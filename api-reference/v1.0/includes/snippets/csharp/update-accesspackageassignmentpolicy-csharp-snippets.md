---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AssignmentPolicie
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"id" , "87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187"
		},
		{
			"displayName" , "All Users"
		},
		{
			"description" , "All users can request for access to the directory."
		},
		{
			"allowedTargetScope" , "allDirectoryUsers"
		},
		{
			"automaticRequestSettings" , null
		},
		{
			"specificAllowedTargets" , new List<>
			{
			}
		},
		{
			"expiration" , new 
			{
				Type = "noExpiration",
			}
		},
		{
			"requestorSettings" , new 
			{
				EnableTargetsToSelfAddAccess = true,
				EnableTargetsToSelfUpdateAccess = false,
				EnableTargetsToSelfRemoveAccess = true,
				AllowCustomAssignmentSchedule = false,
				EnableOnBehalfRequestorsToAddAccess = false,
				EnableOnBehalfRequestorsToUpdateAccess = false,
				EnableOnBehalfRequestorsToRemoveAccess = false,
				OnBehalfRequestors = new List<>
				{
				},
			}
		},
		{
			"requestApprovalSettings" , new 
			{
				IsApprovalRequiredForAdd = true,
				IsApprovalRequiredForUpdate = false,
				Stages = new List<>
				{
					new 
					{
						DurationBeforeAutomaticDenial = "P2D",
						IsApproverJustificationRequired = false,
						IsEscalationEnabled = false,
						DurationBeforeEscalation = "PT0S",
						PrimaryApprovers = new List<>
						{
							new 
							{
								OdataType = "#microsoft.graph.requestorManager",
								ManagerLevel = 1,
							},
						},
						FallbackPrimaryApprovers = new List<>
						{
							new 
							{
								OdataType = "#microsoft.graph.singleUser",
								UserId = "e6bf4d7d-6824-4dd0-809d-5bf42d4817c2",
								Description = "user",
							},
						},
						EscalationApprovers = new List<>
						{
						},
						FallbackEscalationApprovers = new List<>
						{
						},
					},
				},
			}
		},
		{
			"accessPackage" , new 
			{
				Id = "49d2c59b-0a81-463d-a8ec-ddad3935d8a0",
			}
		},
	},
};
await graphClient.IdentityGovernance.EntitlementManagement.AssignmentPolicies["accessPackageAssignmentPolicy-id"].PutAsync(requestBody);


```