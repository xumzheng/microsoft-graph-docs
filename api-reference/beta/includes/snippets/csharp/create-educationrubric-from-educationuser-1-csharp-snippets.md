---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EducationRubric
{
	DisplayName = "Example Credit Rubric",
	Description = new EducationItemBody
	{
		Content = "This is an example of a credit rubric (no points)",
		ContentType = "text",
	},
	Levels = new List<RubricLevel>
	{
		new RubricLevel
		{
			DisplayName = "Good",
			Description = new EducationItemBody
			{
				Content = "",
				ContentType = "text",
			},
		},
		new RubricLevel
		{
			DisplayName = "Poor",
			Description = new EducationItemBody
			{
				Content = "",
				ContentType = "text",
			},
		},
	}
	Qualities = new List<RubricQuality>
	{
		new RubricQuality
		{
			Description = new EducationItemBody
			{
				Content = "Argument",
				ContentType = "text",
			},
			Criteria = new List<RubricCriterion>
			{
				new RubricCriterion
				{
					Description = new EducationItemBody
					{
						Content = "The essay's argument is persuasive.",
						ContentType = "text",
					},
				},
				new RubricCriterion
				{
					Description = new EducationItemBody
					{
						Content = "The essay's argument does not make sense.",
						ContentType = "text",
					},
				},
			}
		},
		new RubricQuality
		{
			Description = new EducationItemBody
			{
				Content = "Spelling and Grammar",
				ContentType = "text",
			},
			Criteria = new List<RubricCriterion>
			{
				new RubricCriterion
				{
					Description = new EducationItemBody
					{
						Content = "The essay uses proper spelling and grammar with few or no errors.",
						ContentType = "text",
					},
				},
				new RubricCriterion
				{
					Description = new EducationItemBody
					{
						Content = "The essay has numerous errors in spelling and/or grammar.",
						ContentType = "text",
					},
				},
			}
		},
	}
};
var result = await graphClient.Education.Me.Rubrics.PostAsync(requestBody);


```