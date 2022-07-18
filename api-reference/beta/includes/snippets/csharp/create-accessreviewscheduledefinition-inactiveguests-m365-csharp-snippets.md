---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessReviewScheduleDefinition
{
	DisplayName = "Review inactive guests on teams",
	DescriptionForAdmins = "Control guest user access to our teams.",
	DescriptionForReviewers = "Information security is everyone's responsibility. Review our access policy for more.",
	InstanceEnumerationScope = new AccessReviewScope
	{
		@odata.type = "#microsoft.graph.accessReviewQueryScope",
		AdditionalData = new()
		{
			{"query", "/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team')')"},
			{"queryType", "MicrosoftGraph"},
		}
	},
	Scope = new AccessReviewScope
	{
		@odata.type = "#microsoft.graph.accessReviewInactiveUsersQueryScope",
		AdditionalData = new()
		{
			{"query", "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')"},
			{"queryType", "MicrosoftGraph"},
			{"inactiveDuration", "P30D"},
		}
	},
	Reviewers = new List<Object>
	{
		new 
		{
			AdditionalData = new()
			{
				{"query", "./owners"},
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
				{"query", "/users/fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f"},
				{"queryType", "MicrosoftGraph"},
			}
		},
	}
	Settings = new AccessReviewScheduleSettings
	{
		MailNotificationsEnabled = true,
		ReminderNotificationsEnabled = true,
		JustificationRequiredOnApproval = true,
		RecommendationsEnabled = true,
		InstanceDurationInDays = 3,
		Recurrence = new PatternedRecurrence
		{
			Pattern = new RecurrencePattern
			{
				Type = "absoluteMonthly",
				DayOfMonth = 5,
				Interval = 3,
			},
			Range = new RecurrenceRange
			{
				Type = "noEnd",
				StartDate = "2020-05-04T00:00:00.000Z",
			},
		},
		DefaultDecisionEnabled = true,
		DefaultDecision = "Deny",
		AutoApplyDecisionsEnabled = true,
	},
};
var result = await graphClient.IdentityGovernance.AccessReviews.Definitions.PostAsync(requestBody);


```