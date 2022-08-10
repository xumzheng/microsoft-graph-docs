---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CustomSecurityAttributeDefinition
{
	AttributeSet = "Engineering",
	Description = "Active projects for user",
	IsCollection = true,
	IsSearchable = true,
	Name = "Project",
	Status = "Available",
	Type = "String",
	UsePreDefinedValuesOnly = true,
	AllowedValues = new List<AllowedValue>
	{
		new AllowedValue
		{
			Id = "Alpine",
			IsActive = true,
		},
		new AllowedValue
		{
			Id = "Baker",
			IsActive = true,
		},
		new AllowedValue
		{
			Id = "Cascade",
			IsActive = true,
		},
	},
};
var result = await graphClient.Directory.CustomSecurityAttributeDefinitions.PostAsync(requestBody);


```