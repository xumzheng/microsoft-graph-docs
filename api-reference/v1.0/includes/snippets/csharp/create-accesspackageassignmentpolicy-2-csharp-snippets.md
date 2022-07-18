---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessPackageAssignmentPolicy
{
	DisplayName = "policy for external access requests",
	Description = "policy for users from connected organizations to request access, with two stages of approval.",
	AllowedTargetScope = "allConfiguredConnectedOrganizationUsers",
	SpecificAllowedTargets = new List<SubjectSet>
	{
	}
	Expiration = new ExpirationPattern
	{
		Type = "noExpiration",
	},
	RequestorSettings = new AccessPackageAssignmentRequestorSettings
	{
		EnableTargetsToSelfAddAccess = true,
		EnableTargetsToSelfUpdateAccess = true,
		EnableTargetsToSelfRemoveAccess = true,
		AllowCustomAssignmentSchedule = false,
		EnableOnBehalfRequestorsToAddAccess = false,
		EnableOnBehalfRequestorsToUpdateAccess = false,
		EnableOnBehalfRequestorsToRemoveAccess = false,
		OnBehalfRequestors = new List<SubjectSet>
		{
		}
	},
	RequestApprovalSettings = new AccessPackageAssignmentApprovalSettings
	{
		IsApprovalRequiredForAdd = true,
		IsApprovalRequiredForUpdate = false,
		Stages = new List<AccessPackageApprovalStage>
		{
			new AccessPackageApprovalStage
			{
				DurationBeforeAutomaticDenial = "P14D",
				IsApproverJustificationRequired = false,
				IsEscalationEnabled = false,
				DurationBeforeEscalation = "PT0S",
				PrimaryApprovers = new List<SubjectSet>
				{
					new SubjectSet
					{
						@odata.type = "#microsoft.graph.internalSponsors",
					},
				}
				FallbackPrimaryApprovers = new List<SubjectSet>
				{
					new SubjectSet
					{
						@odata.type = "#microsoft.graph.singleUser",
						AdditionalData = new()
						{
							{"userId", "7deff43e-1f17-44ef-9e5f-d516b0ba11d4"},
						}
					},
					new SubjectSet
					{
						@odata.type = "#microsoft.graph.groupMembers",
						AdditionalData = new()
						{
							{"groupId", "1623f912-5e86-41c2-af47-39dd67582b66"},
						}
					},
				}
				EscalationApprovers = new List<SubjectSet>
				{
				}
				FallbackEscalationApprovers = new List<SubjectSet>
				{
				}
			},
			new AccessPackageApprovalStage
			{
				DurationBeforeAutomaticDenial = "P14D",
				IsApproverJustificationRequired = false,
				IsEscalationEnabled = false,
				DurationBeforeEscalation = "PT0S",
				PrimaryApprovers = new List<SubjectSet>
				{
				}
				FallbackPrimaryApprovers = new List<SubjectSet>
				{
					new SubjectSet
					{
						@odata.type = "#microsoft.graph.singleUser",
						AdditionalData = new()
						{
							{"userId", "46184453-e63b-4f20-86c2-c557ed5d5df9"},
						}
					},
					new SubjectSet
					{
						@odata.type = "#microsoft.graph.groupMembers",
						AdditionalData = new()
						{
							{"groupId", "1623f912-5e86-41c2-af47-39dd67582b66"},
						}
					},
				}
				EscalationApprovers = new List<SubjectSet>
				{
				}
				FallbackEscalationApprovers = new List<SubjectSet>
				{
				}
			},
		}
	},
	ReviewSettings = new AccessPackageAssignmentReviewSettings
	{
		IsEnabled = true,
		ExpirationBehavior = "keepAccess",
		IsRecommendationEnabled = true,
		IsReviewerJustificationRequired = true,
		IsSelfReview = false,
		Schedule = new EntitlementManagementSchedule
		{
			StartDateTime = DateTimeOffset.Parse("2022-07-02T06:59:59.998Z"),
			Expiration = new ExpirationPattern
			{
				Duration = "P14D",
				Type = "afterDuration",
			},
			Recurrence = new PatternedRecurrence
			{
				Pattern = new RecurrencePattern
				{
					Type = "absoluteMonthly",
					Interval = 3,
					Month = 0,
					DayOfMonth = 0,
					DaysOfWeek = new List<DayOfWeek>
					{
					}
				},
				Range = new RecurrenceRange
				{
					Type = "noEnd",
					NumberOfOccurrences = 0,
				},
			},
		},
		PrimaryReviewers = new List<SubjectSet>
		{
			new SubjectSet
			{
				@odata.type = "#microsoft.graph.groupMembers",
				AdditionalData = new()
				{
					{"groupId", "1623f912-5e86-41c2-af47-39dd67582b66"},
				}
			},
		}
		FallbackReviewers = new List<SubjectSet>
		{
		}
	},
	AccessPackage = new 
	{
		Id = "a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b",
	},
};
var result = await graphClient.IdentityGovernance.EntitlementManagement.AssignmentPolicies.PostAsync(requestBody);


```