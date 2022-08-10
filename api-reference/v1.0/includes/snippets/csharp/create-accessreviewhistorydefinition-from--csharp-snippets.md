---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessReviewHistoryDefinition
{
	DisplayName = "Last quarter's group reviews April 2021",
	Decisions = new List<>
	{
		"approve",
		"deny",
		"dontKnow",
		"notReviewed",
		"notNotified",
	},
	ScheduleSettings = new AccessReviewHistoryScheduleSettings
	{
		ReportRange = "P1M",
		Recurrence = new PatternedRecurrence
		{
			Pattern = new RecurrencePattern
			{
				Type = RecurrencePatternType.Monthly,
				Interval = 1,
			},
			Range = new RecurrenceRange
			{
				Type = RecurrenceRangeType.Noend,
				StartDate = "2018-08-03T21:02:30.667Z",
				AdditionalData = new Dictionary<string, object>
				{
					{
						"count" , 0
					},
				},
			},
		},
	},
	Scopes = new List<AccessReviewScope>
	{
		new AccessReviewScope
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"@odata.type" , "#microsoft.graph.accessReviewQueryScope"
				},
				{
					"queryType" , "MicrosoftGraph"
				},
				{
					"query" , "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')"
				},
				{
					"queryRoot" , null
				},
			},
		},
		new AccessReviewScope
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"@odata.type" , "#microsoft.graph.accessReviewQueryScope"
				},
				{
					"queryType" , "MicrosoftGraph"
				},
				{
					"query" , "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')"
				},
				{
					"queryRoot" , null
				},
			},
		},
	},
};
var result = await graphClient.IdentityGovernance.AccessReviews.HistoryDefinitions.PostAsync(requestBody);


```