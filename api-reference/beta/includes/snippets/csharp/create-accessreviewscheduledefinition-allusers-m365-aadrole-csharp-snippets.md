---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessReviewScheduleDefinition
{
	DisplayName = "Review employee access to LinkedIn",
	DescriptionForAdmins = "Review employee access to LinkedIn",
	Scope = new AccessReviewScope
	{
		@odata.type = "#microsoft.graph.principalResourceMembershipsScope",
		AdditionalData = new()
		{
			{"principalScopes", new List<Object>
			{
			}
			{"resourceScopes", new List<Object>
			{
			}
		}
	},
	Reviewers = new List<Object>
	{
		new 
		{
			AdditionalData = new()
			{
				{"query", "./manager"},
				{"queryType", "MicrosoftGraph"},
				{"queryRoot", "decisions"},
			}
		},
	}
	BackupReviewers = new List<Object>
	{
		new 
		{
			AdditionalData = new()
			{
				{"query", "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers"},
				{"queryType", "MicrosoftGraph"},
			}
		},
	}
	FallbackReviewers = new List<Object>
	{
		new 
		{
			AdditionalData = new()
			{
				{"query", "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers"},
				{"queryType", "MicrosoftGraph"},
			}
		},
	}
	Settings = new AccessReviewScheduleSettings
	{
		MailNotificationsEnabled = true,
		ReminderNotificationsEnabled = true,
		JustificationRequiredOnApproval = true,
		DefaultDecisionEnabled = true,
		DefaultDecision = "Recommendation",
		InstanceDurationInDays = 180,
		AutoApplyDecisionsEnabled = true,
		RecommendationsEnabled = true,
		Recurrence = new PatternedRecurrence
		{
			Pattern = new RecurrencePattern
			{
				Type = "absoluteMonthly",
				Interval = 6,
				DayOfMonth = 0,
			},
			Range = new RecurrenceRange
			{
				Type = "numbered",
				StartDate = "2021-05-05",
				EndDate = "2022-05-05",
			},
		},
	},
};
var result = await graphClient.IdentityGovernance.AccessReviews.Definitions.PostAsync(requestBody);


```