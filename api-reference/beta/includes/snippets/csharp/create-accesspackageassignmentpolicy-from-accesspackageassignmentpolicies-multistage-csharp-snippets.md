---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessPackageAssignmentPolicy
{
	AccessPackageId = "string (identifier)",
	DisplayName = "Users from connected organizations can request",
	Description = "Allow users from configured connected organizations to request and be approved by their sponsors",
	CanExtend = false,
	DurationInDays = 365,
	ExpirationDateTime = null,
	RequestorSettings = new RequestorSettings
	{
		ScopeType = "AllExistingConnectedOrganizationSubjects",
		AcceptRequests = true,
		AllowedRequestors = new List<UserSet>
		{
		}
	},
	RequestApprovalSettings = new ApprovalSettings
	{
		IsApprovalRequired = true,
		IsApprovalRequiredForExtension = false,
		IsRequestorJustificationRequired = true,
		ApprovalMode = "Serial",
		ApprovalStages = new List<ApprovalStage>
		{
			new ApprovalStage
			{
				ApprovalStageTimeOutInDays = 14,
				IsApproverJustificationRequired = true,
				IsEscalationEnabled = true,
				EscalationTimeInMinutes = 11520,
				PrimaryApprovers = new List<UserSet>
				{
					new UserSet
					{
						@odata.type = "#microsoft.graph.groupMembers",
						IsBackup = true,
						AdditionalData = new()
						{
							{"id", "string (identifier)"},
							{"description", "group for users from connected organizations which have no external sponsor"},
						}
					},
					new UserSet
					{
						@odata.type = "#microsoft.graph.externalSponsors",
						IsBackup = false,
					},
				}
				EscalationApprovers = new List<UserSet>
				{
					new UserSet
					{
						@odata.type = "#microsoft.graph.singleUser",
						IsBackup = true,
						AdditionalData = new()
						{
							{"id", "string (identifier)"},
							{"description", "user if the external sponsor does not respond"},
						}
					},
				}
			},
			new ApprovalStage
			{
				ApprovalStageTimeOutInDays = 14,
				IsApproverJustificationRequired = true,
				IsEscalationEnabled = true,
				EscalationTimeInMinutes = 11520,
				PrimaryApprovers = new List<UserSet>
				{
					new UserSet
					{
						@odata.type = "#microsoft.graph.groupMembers",
						IsBackup = true,
						AdditionalData = new()
						{
							{"id", "string (identifier)"},
							{"description", "group for users from connected organizations which have no internal sponsor"},
						}
					},
					new UserSet
					{
						@odata.type = "#microsoft.graph.internalSponsors",
						IsBackup = false,
					},
				}
				EscalationApprovers = new List<UserSet>
				{
					new UserSet
					{
						@odata.type = "#microsoft.graph.singleUser",
						IsBackup = true,
						AdditionalData = new()
						{
							{"id", "string (identifier)"},
							{"description", "user if the internal sponsor does not respond"},
						}
					},
				}
			},
		}
	},
	AccessReviewSettings = new AssignmentReviewSettings
	{
		IsEnabled = true,
		RecurrenceType = "quarterly",
		ReviewerType = "Self",
		StartDateTime = DateTimeOffset.Parse("2020-04-01T07:59:59.998Z"),
		DurationInDays = 25,
		Reviewers = new List<UserSet>
		{
		}
	},
};
var result = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentPolicies.PostAsync(requestBody);


```